# What Are Variables?

In simple terms, let's demystify what variables are without getting too technical. Think of a variable as a box that can hold information, like numbers or words. Just like in math, where we use "X" and "Y" to represent numbers, you can use variables in programming to store and work with data.

So, whether you're using Python, Java, or any other programming language, remember that variables are like your personal containers, ready to hold and handle data.

<div style="text-align:center;">
    <img src="../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Var-Example.webp" alt="Variable Example">
</div>


---

## How to Create and Use Variables in Python

Creating variables in Python is a fundamental skill. In Python, you can store various types of data, such as numbers and words, in variables. This guide will walk you through the basics of creating and using variables, including data types.

### Storing Values in Variables

In Python, you can assign values to variables using a simple syntax. Let's look at some examples:

```python
x = 53  # We're storing the number 53 in the variable x
y = "John"  # Here, we're storing the word "John" in the variable y

print(x, y)  # Using the print function, you can see the contents of x and y.
```

See how we didn't have to specify that the first line is an integer or the second is a string.

That is Because Python is dynamic, which means you don't need to specify a data type when creating a variable. It also executes code line by line. If you assign different data types to the same variable, the last assignment takes precedence. For instance:

```python
x = 53
x = "John"

print(x)
```

This will only print `John` and ignore the first line, `53`.

### Checking Variable Data Types

Sometimes, you may want to know the data type of a variable in your code. To do this, you can use the built-in function `type`. Here's an example:

```python
x = "John"
y = 53
print(type(x))
print(type(y))
```

this code will print out

```terminal
<class 'str'>
<class 'int'>
```

### Choosing Single or Double Quotation Marks

In Python, you can use either single or double quotation marks to create strings. It's a matter of personal preference; choose the style that suits you.

### Explicitly Specifying Data Types

While Python is dynamic, you can explicitly specify a data type when assigning a value to a variable. This helps Python understand how to handle the data. Here's how it's done:

```python
x = str(53)    # x is a string containing the number 53
y = int(53)    # y is an integer holding the value 53
z = float(53)  # z is a floating-point number with the value 53.0
```

In this code, we're using `str()`, `int()`, and `float()` to explicitly define the data type of the variable and assign a value to it. This can be useful when you want to make sure your program interprets the data correctly.

----

## How to Create Variable Names?

Think of it as naming your pets; you want something that makes sense and is easy to remember. In Python, you've got quite a bit of freedom, but there are some ground rules and suggestions that you should know.

1. **Start with a Letter or Underscore**

    Imagine naming your dog "123Fido" - it just doesn't work, right? Well, variable names in Python are similar. They must always kick off with a letter (either uppercase or lowercase) or an underscore (_). No numbers allowed at the beginning!

    For example:

    ```python
    name = "John"
    _age = 53
    ```

2. **Use Letters, Numbers, and Underscores**

    Here's a twist: while you can't start with a number, you can certainly use them in your variable names. Just don't go crazy with special characters like @, $, %, and others. Spaces? Nope, Python doesn't like those either!

    For example:

    ```python
    _name = "John"
    ag3 = 53
    last_name = "Dough"
    ```

3. **Python Is a Stickler for Case**

    Python pays close attention to capitalization. It's like having two pets with similar names - "`myName`" and "`myname`" are different in Python's eyes. So, "`myName`" and "`myname`" are two separate variables.

    For example:

    ```python
    myName = "John"
    myname = "Dough"
    ```

4. **Be Descriptive with Names**

    Imagine if you named your fish "F" instead of "Fluffy the Fish." You'd have no idea which one is which! The same goes for variable names. Use names that tell you or anyone reading your code what the variable is all about.

    For instance:

    ```python
    john_age = 53
    ```

    *That's way better than using "ts" to represent a total score, right?*

5. Avoid Python Keywords

    Python has a list of special words reserved for its own purposes, like "`if`," "`else`," "`while`," and "`for`." Don't try to use these words as variable names. It's like trying to name your pet "If" - it just won't work!

    For example ( don't ever do this lol):

    ```python
    if = 5  # This is not allowed
    ```

6. Stick to Lowercase Letters

    In Python, it's common to write variable names in lowercase letters and separate words with underscores. This style is called "`snake_case`." It's like naming your pets with names like "*dog_buddy*" or "*cat_whiskers*."

    For example:

    ```python
    student_name = "Alice"
    ```

    While some people prefer "`camelCase`" (writing variable names like "userAge"), it's less common in Python. So, it's better to stick with "`snake_case`" for consistency. Ultimately, it all comes down to personal preference, in my opinion.

---

## Assigning Multiple Values to Variables in Python

Python makes it easy to assign values to multiple variables in a single line of code. This can be a helpful concept when you want to work with several pieces of data simultaneously. Let's explore this with some real-world examples and code.

```python
Friend_1, Friend_2, Friend_3 = "Candy_1", "Candy_2", "Candy_3"
print(Friend_1)
print(Friend_2)
print(Friend_3)
```

*In this example, we have three variables: Friend_1, Friend_2, and Friend_3, each representing a friend's favorite candy. When you execute this code, it will display the favorite candy of each friend: Friend_1 loves "Candy_1," Friend_2 enjoys "Candy_2," and Friend_3 prefers "Candy_3."*

It's crucial to ensure that the number of variables on the left side of the assignment matches the number of values on the right side; otherwise, you will encounter an error. This Python feature is particularly useful for initializing multiple variables succinctly and can be employed in various scenarios, such as data processing and unpacking values from data structures like tuples and lists.

### Error - Mismatched Values and Variables

```python
alice, bob, carol = "Chocolate", "Gummy Bears"
print(alice)
print(bob)
print(carol)
```

**Error Explanation:**

In this code, we have attempted to assign values to three variables (alice, bob, and carol) while providing only two values: "Chocolate" and "Gummy Bears."

Python expects the number of variables on the left side of the assignment to match the number of values on the right side. In this case, we have three variables but only two values. When you run this code, you will encounter a ValueError with a message similar to something like this:

```terminal
ValueError: not enough values to unpack (expected 3, got 2)
```

The error message tells us that Python expected three values but received only two. To fix this error, you should provide the correct number of values to match the number of variables, like so:

```python
alice, bob, carol = "Chocolate", "Gummy Bears", "Lollipops"
print(alice)
print(bob)
print(carol)
```

This corrected code assigns "Chocolate" to alice, "Gummy Bears" to bob, and "Lollipops" to carol, ensuring that there are enough values for each variable, and it will run without errors.

---

## Output Variables Guide

In Python, when you write programs, you often want to show information to the person using your program. You can think of it like talking to the computer and asking it to show you something. To do this, we use a special tool called the print() function.

If you want to learn more about the print() function and how to use it, you can check out the discussion I had on this topic in a different file, "Hello World" [**Click Here**](c.%20Hello%20World.md).

### Displaying a Single Variable

Imagine you have a piece of information, like a name. You want to see that name on your computer screen. To do this, you can use the print() function. Here's how you can show a name using it:

```python
name = "Alice"
print(name)
```

When you run this code, it will show "Alice" on the screen. It's like telling Python, "Hey, please show me what's inside the name box."

### Displaying Multiple Variables

Sometimes, you have more than one thing you want to show. For example, let's say you have three numbers: 2, 4, and 6. You can show all of them using the print() function and separate them with commas like this:

```python
num1 = 2
num2 = 4
num3 = 6
print(num1, num2, num3)
```

When you run this code, it will display "2 4 6" on the screen, with spaces between the numbers. So, print(num1, num2, num3) is like saying, "Python, please show me the values of num1, num2, and num3, and put spaces between them."

### Combining Text Variables

Sometimes, you want to put words together. Let's say you have a first name and a last name, and you want to display the full name. You can do that by combining the text from both variables using the + operator:

```python
first_name = "John"
last_name = "Smith"
full_name = first_name + " " + last_name
print(full_name)
```

Here, first_name + " " + last_name combines the text from first_name and last_name and displays "John Smith" on the screen. Notice the space in " ", which ensures there's a space between the first and last name.

### Adding Numbers

If you have numbers and you want to add them together, you can use the + operator:

```python
num1 = 7
num2 = 3
result = num1 + num2
print(result)
```

When you run this code, it will display "10" because num1 + num2 is like asking Python to add 7 and 3 together.

### Be Careful with Mixing Text and Numbers

But be cautious! If you try to mix numbers and text using the + operator, Python might get confused:

```python
age = 25
message = "I am " + age + " years old."
print(message)
```

In this case, Python doesn't understand how to add a number (age) and text together, so it would give you an error.

### The Best Way

To avoid confusion, it's safest to use commas when using the print() function. This way, you can even mix different types of information:

```python
age = 25
message = "I am", age, "years old."
print(message)
```

When you run this code, it will display "I am 25 years old." Using commas tells Python, "Show me both the text and the value of age."

#### That's how you can easily show your information in Python using the print() function! 

---

## Exploring Output-Related Variables



---

## Understanding Global Variables in Python



---

[![Previous Page](https://img.shields.io/badge/Previous%20Page-0077B5?style=for-the-badge)](./d.%20Comments.md)
[![Next Page](https://img.shields.io/badge/Next%20Page-1DA1F2?style=for-the-badge)](./f.%20Data%20Types.md)
