# Basic Input & Output (I/O) Tutorial for Beginners

When you're just starting with Python, it's essential to learn how to request information from users and display that information as output. In this tutorial, we will cover printing output using the print() function, formatting output using f-strings and str.format(), obtaining input from users using the input() function, and exploring some real-life examples for better understanding.

## Getting User Input()

Imagine the `input()` function as a means for your Python program to have in a conversation with users. It serves as a bridge that enables your program to ask questions, and users can respond to that. You can use it to collect various types of information, such as names, numbers, or even special characters, and then store that information in a variable ([Learn more about Variables](./e.%20Python%20Variables.md)).

### Example: Asking for the User's Name

Let's begin with a very basic example. We'll use the `input()` function to ask the user for their name and then store what they type in a variable `name`. 

```python
name = input("What is your name: ")
```

_Note: Pay attention to the space after the text in double quotes ("What is your name: ") in the code above. If you forget to add that space, there won't be a space after the question, which might confuse the user._

What the above program does is ask for the user's name and store it in the `name` variable for us to use later in the code.

Now, in the same code, let's use print to output the name we asked from the user.

Here's how you do it:

```python
# Get user's name
name = input("What is your name: ")

# Display the user's name
print("Hello, " + name + "!")
```

Output:

```terminal
What is your name: Sajid
Hello, Sajid!
>
```

In this example, the program asks the user for their name, and when the user enters "Sajid," it greets them with "Hello, Sajid!" using the `print()` function. This demonstrates the basics of obtaining user input and displaying output in Python.