# What Are Variables?

In simple terms, let's demystify what variables are without getting too technical. Think of a variable as a box that can hold information, like numbers or words. Just like in math, where we use "X" and "Y" to represent numbers, you can use variables in programming to store and work with data.

So, whether you're using Python, Java, or any other programming language, remember that variables are like your personal containers, ready to hold and handle data.

<div style="text-align:center;">
    <img src="../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Var-Example.webp" alt="Variable Example">
</div>

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

## How to Assign Variable Names in Python

Choosing a variable name might sound as easy as naming your pet goldfish, but in Python, there are some rules to follow. Don't worry; we'll keep it simple and fun!
