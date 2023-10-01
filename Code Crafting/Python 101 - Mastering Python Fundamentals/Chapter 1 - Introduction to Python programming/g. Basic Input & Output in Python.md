# Basic Input & Output (I/O) Tutorial for Beginners

When you're just starting with Python, it's essential to learn how to request information from users and display that information as output. In this tutorial, you'll learn how to interact with users by getting input from them and displaying information as output. This fundamental skill is essential for creating interactive programs.

## Getting User Input

Imagine the `input()` function as a means for your Python program to have a conversation with the users. It serves as a bridge that enables your program to ask questions, and users can respond to that. You can use it to collect various types of information, such as names, numbers, or even special characters, and then store that information for later use.

### Example: Getting User Input and Saying Hello

Let's begin with a very basic example. We'll use the `input()` function to ask the user for their name and then store what they type in a variable `name`. 

```python
# Get the user's name
name = input("What is your name: ")
```

When you run this program, it will display the question "What is your name: ". You can type your name as a response, and the program will save it in the name [variable](./e.%20Python%20Variables.md).

Now, let's use the `print()` function to say hello using the name we obtained:

```python
# Get the user's name
name = input("What is your name: ")

# Say hello using the user's name
print("Hello, " + name + "!")
```
When you run this code, it will ask for your name, and after you provide it, it will greet you with "Hello, [your name]!"

Output:

```terminal
> What is your name: Sajid
> Hello, Sajid!
> _
```

Congratulations! You've just learned how to get input from users and display output in Python. These are the basic building blocks for creating interactive programs. You can use these skills to make your Python programs more engaging and user-friendly.

Remember, it's okay to start with simple examples like this one. As you become more comfortable, you can explore more advanced input and output techniques. Happy coding!

## 📚 Further Learning Resources

1. Python Docs (Documentation) - [Advanced Input & Output](https://docs.python.org/3/tutorial/inputoutput.html)
2. Input & Output Code (W3Schools) - [Example 1](https://www.w3schools.com/python/showpython.asp?filename=demo_ref_input) & [Example 2](https://www.w3schools.com/python/showpython.asp?filename=demo_ref_input2)
3. More Input and Output Method (GeeksforGeeks) - [Advanced Concepts](https://www.geeksforgeeks.org/input-and-output-in-python/)

## Page Navigation

[![Previous Page](https://img.shields.io/badge/Previous%20Page-0077B5?style=for-the-badge)](./f.%20Demystifying%20Data%20Types%20.md)
[![Next Page](https://img.shields.io/badge/Next%20Page-1DA1F2?style=for-the-badge)](#)
