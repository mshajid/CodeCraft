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

## Assigning Multiple Values to Variables in Python

If you thought Python only lets you assign one piece of data to each variable, get ready for a surprise! Python allows you to assign multiple values to a single variable ( [Click Here to Learn about dictionaries in Python](<../../../Quick Reference/What's a Python Dictionary.md>) ), and it even supports different data types for these values.

<!--- have more to add --->


## Output Variables

## Understanding Output-Related Variables

## Exploring Global Variables

[![Previous Page](https://img.shields.io/badge/Previous%20Page-0077B5?style=for-the-badge)](./d.%20Comments.md)
[![Next Page](https://img.shields.io/badge/Next%20Page-1DA1F2?style=for-the-badge)](./f.%20Data%20Types.md)
