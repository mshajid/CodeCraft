# What is an API

**API**, or **Application Programming Interface**, is a set of rules and protocols that allows one software application to interact with another. It defines the methods and data formats that applications can use to request and exchange information seamlessly. Think of it as the menu and order system in a restaurant; you, the customer (or application), don't need to understand how the kitchen (or another application) prepares your meal (data), but you can place an order (send a request) through the waiter (API), and your dish (data) will be served.

![API EXAMPLE with Cx Waiter and Chef](../Assets/Quick%20Reference/What%20is%20an%20API/API%20Example.jpg)

## Types of APIs

There are various types of APIs, each designed for specific purposes and use cases. Here are some common types:

1. **Web APIs (RESTful APIs)**: These are the most prevalent types of APIs on the internet. Web APIs use HTTP requests to enable communication over the web. They typically follow the principles of Representational State Transfer (REST) and provide a structured way to access resources, such as retrieving data from a database, updating information, or performing other actions over the internet.

    ```python
    import requests

    # Get the latitude and longitude of the Eiffel Tower
    response = requests.get('https://maps.googleapis.com/maps/api/geocode/json?address=Eiffel+Tower&key=API_KEY_GOES_HERE')

    # Parse the JSON response
    data = response.json()

    # Get the latitude and longitude
    latitude = data['results'][0]['geometry']['location']['lat']
    longitude = data['results'][0]['geometry']['location']['lng']

    # Print the latitude and longitude
    print(latitude)
    print(longitude)

    ```

2. **SOAP APIs**: Simple Object Access Protocol (SOAP) is a protocol-based API that uses XML as a messaging format. SOAP APIs are known for their strict standards and are often used in enterprise-level applications for their robustness and security features.

    ```python
    import requests
    from suds.client import Client

    # Create a SOAP client
    client = Client('https://ec2.amazonaws.com/wsdl/2016-11-15/ec2.wsdl')

    # Get a list of running EC2 instances
    response = client.service.DescribeInstances()

    # Parse the SOAP response
    instances = response.reservationSet.reservation[0].instancesSet.item

    # Print the instance IDs
    for instance in instances:
        print(instance.instanceId)
    ```

3. **GraphQL APIs**: GraphQL is a query language for APIs that allows clients to request only the data they need. Unlike RESTful APIs, where the server determines the data structure in responses, GraphQL APIs put the control in the hands of the client, allowing more flexibility and efficiency in data retrieval.

    ```python
    import requests

    # Query the GitHub API to get a list of the most starred repositories
    query = """
    query {
    repositories(orderBy: {field: STARGAZERS_COUNT, direction: DESC}, first: 100) {
        nodes {
        name
        stargazersCount
        }
    }
    }
    """

    # Make a GraphQL request
    response = requests.post('https://api.github.com/graphql', json={'query': query})

    # Parse the JSON response
    data = response.json()

    # Print the names of the most starred repositories
    for repository in data['data']['repositories']['nodes']:
        print(repository['name'])
    ```

4. **Library or SDK APIs**: These APIs are provided as libraries or software development kits (SDKs) that developers can integrate into their applications. These libraries abstract complex operations and provide pre-built functions or classes, making it easier to interact with specific services or functionalities.

    ```python
    import twilio

    # Create a Twilio client
    client = twilio.rest.Client('YOUR_ACCOUNT_SID', 'YOUR_AUTH_TOKEN')

    # Send a text message
    message = client.messages.create(
        body='Hello, world!',
        to='+15555555555',
        from_='+14155555555'
    )

    # Print the message ID
    print(message.sid)
    ```

5. **Hardware APIs**: These APIs allow software to communicate with hardware devices, such as sensors, cameras, or printers. They provide a standardized way for applications to access and control hardware components.

    ```python
    import board
    import pwmio

    # Create a PWM object
    pwm = pwmio.PWMOut(board.D18)

    # Set the PWM frequency to 50 Hz
    pwm.frequency = 50

    # Set the PWM duty cycle to 50%
    pwm.duty_cycle = 50

    # Start the PWM output
    pwm.start()
    ```

6. **Database APIs**: Database APIs, often known as Database Management System (DBMS) APIs, enable software applications to connect to and interact with databases. They provide functions for querying, updating, and managing data stored in a database system.

    ```python
    import mysql.connector

    # Connect to the MySQL database
    connection = mysql.connector.connect(
        host='localhost',
        user='root',
        password='password',
        database='my_database'
    )

    # Create a cursor
    cursor = connection.cursor()

    # Execute a SQL query
    cursor.execute('SELECT * FROM users')

    # Get the results of the query
    results = cursor.fetchall()

    # Print the results
    for result in results:
        print(result)

    # Close the cursor and connection
    cursor.close()
    connection.close()
    ```

7. **Operating System APIs**: These APIs provide access to various operating system features and services. They allow applications to interact with the file system, manage processes, control hardware peripherals, and more.

    ```python
    import os

    # Get the current working directory
    cwd = os.getcwd()

    # Print the current working directory
    print(cwd)

    # Change the current working directory
    os.chdir('/home/user')

    # Get the new current working directory
    cwd = os.getcwd()

    # Print the new current working directory
    print(cwd)
    ```

## Why APIs are Used

APIs serve several essential purposes in software development and modern computing:

1. **Modularity**: APIs allow developers to split big software projects into smaller, easier-to-manage pieces. This makes it simpler for different teams to work on different parts of a project at the same time.

2. **Interoperability**: APIs let different software, even if they're made by different companies, understand each other and work together smoothly. This helps different apps or systems cooperate and share information.

3. **Reusability**: Instead of building everything from scratch, developers can reuse existing APIs like building blocks. This saves time and reduces mistakes because they can rely on tried-and-tested code.

4. **Scalability**: APIs make it easy to add new features or services to a program without messing up what's already there. This is super important as technology keeps changing and evolving.

5. **Security**: APIs help keep things safe. They can make sure only the right people or programs can access sensitive information or do important tasks.

6. **Third-Party Integration**: Developers often use APIs to add cool features to their apps without building them from scratch. For example, you can use APIs to put a map into your app, let users pay with a credit card, or share stuff on social media. It's like adding extra functions to your app without reinventing the wheel.

## Practical Example

For this example, were going to create a simple API code in Python using the Flask framework illustrates how an API can be created and used. In this example, we will create a basic RESTful API for managing a list of tasks.

```python
from flask import Flask, jsonify, request

app = Flask(__name__)

# Sample list of tasks (initially empty)
tasks = []

# Define an API endpoint to add a new task
@app.route('/add_task', methods=['POST'])
def add_task():
    try:
        data = request.get_json()
        task_name = data.get('task_name')
        if task_name:
            tasks.append(task_name)
            return jsonify({'message': 'Task added successfully'}), 201
        else:
            return jsonify({'error': 'Task name is required'}), 400
    except Exception as e:
        return jsonify({'error': str(e)}), 500

# Define an API endpoint to get all tasks
@app.route('/get_tasks', methods=['GET'])
def get_tasks():
    try:
        return jsonify({'tasks': tasks})
    except Exception as e:
        return jsonify({'error': str(e)}), 500

if __name__ == '__main__':
    app.run(debug=True)
```

_To use this code snippet, simply copy it into a new file called app.py and save it. Then, open a terminal and navigate to the directory where you saved the file. Run the following command to start the Flask development server:_
`python app.py`

_Your API will now be running on http://localhost:5000. You can use curl or Postman to send requests to the API endpoints._

### How This Code Works

In this code, we have created a basic Flask web application with two API endpoints:

1. `/add_task` (POST): This endpoint allows you to add a new task to the tasks list. You send a JSON request with the task_name, and the server adds it to the list.

2. `/get_tasks` (GET): This endpoint retrieves and returns the list of tasks as JSON.

### Now, let's explain how to use these APIs:

**Adding a Task:** If you want to add a new task, you can tell our program by sending it a special message. You can do this using a tool like Postman or a command called "curl." When you send this message, you need to include the name of the task you want to add.

For example, you can send a message like this:

```json
{
    "task_name": "Buy groceries"
}
```

After you send this message, our program will reply and tell you if it added the task successfully or if there was a problem. You'll get a message like this:


```json
{
  "message": "Task added successfully"
}
```

**Getting Tasks:**  If you want to see the list of tasks we have, you can ask our program for that list. You do this by sending another kind of message.

When you send this message, our program will reply with the list of tasks in a format that's easy for computers to understand. It looks something like this:

```json
{
  "tasks": [
    "Do laundry",
    "Go to the grocery store",
    "Clean the house"
  ]
}
```

So, you can use these two parts of our program to add tasks and check the list of tasks whenever you want.

## Conclusion

In summary, APIs, or Application Programming Interfaces, are like bridges that enable different software systems to communicate and work together seamlessly. They come in various types to suit different needs and purposes, making them a fundamental part of modern software development.

Through the practical example provided, you've seen how APIs can be applied in real-world scenarios to create and use web services, making tasks like managing to-do lists more accessible and efficient. As you delve deeper into the world of programming, understanding APIs and how to work with them will become a valuable skill for building powerful and interconnected software applications.
