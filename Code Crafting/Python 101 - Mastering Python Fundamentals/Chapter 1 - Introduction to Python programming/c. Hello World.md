# Hello World in Python: A Beginner's Guide

## Writing Code in the Command Line: Script Mode

Before you start writing code in Visual Studio Code or any other text editor, let's begin by writing some lines of code in your terminal or Command Prompt (CMD) to get started.

### Opening the Terminal or CMD

To open the terminal or CMD on your computer, follow these steps:

1. Press the Windows key on your keyboard.
2. Type `cmd` or `Command Prompt`.
3. Press Enter.

You should now see a window open that looks like this:

<img src="../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/CMD.png" alt="Command Prompt" width="500">

### Starting Python Mode

In the terminal or CMD, type the word `python` and then press Enter.

When you do this, your terminal will enter "Python Mode." In simple terms, typing "python" in your terminal invokes the Python interpreter, which allows you to write Python code.

### Understanding the Terminal

Before we write some lines of code, let's understand the elements in the terminal:

![Python Shell](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Python-Terminal.png)
"I am using a cloud shell to demonstrate, but even in CMD or Terminal, it should look the same."

- **Red Arrow**: This arrow indicates where you typed the word `Python` to invoke the interpreter.

- **Green Line**: The green line shows where to check for the Python version when you invoke this language interpreter. the current latest version is 3.11.5.

- **Yellow Arrow**: The three white `>>>` symbols indicate where you need to type the Python prompt. This is where you should write your code.

### Writing "Hello, World" in the Terminal

Now, let's type our first line of code, which is "Hello, World," in the terminal:

![Hello World](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Hello-WORLD-CLI.png)

In the terminal, type the following code and press Enter:

    print("Hello, World")

This line of code is quite self-explanatory. We are instructing the interpreter to "Print this line of text in the terminal." After typing this line of code and pressing Enter, it should print out "Hello, World" in the terminal:

![Hello World](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Hello-World-print.png)

Congratulations! You've just written and executed your first Python program in the terminal. This is a simple but important step as you begin your journey into Python programming.

## Writing "Hello, World" in an IDE (VSCode)

Now that we've executed our first lines of code in the terminal, let's do the same thing using an Integrated Development Environment (IDE). We'll be using VSCode for this.

If you haven't installed VS Code yet, you can follow this tutorial I've prepared on how to install it:

| Tutorial Link                                                     | Description                                        |
| ----------------------------------------------------------------- | -------------------------------------------------- |
| [🚀 Click Here](../../../Before%20You%20Start/2.%20Dev-Tools%20Setup%20Guide.md) | Setting Up Development Tools                      |
| [⚙️ Click Here](../../../Before%20You%20Start/3.%20Workspace%20Setup%20Guide.md) | Setting Up Your Workspace in VSCode                |

If you already have VSCode or any other IDE installed, you can proceed with the following steps to write and run your code in a text editor.

Open VS Code and create a new file by typing the following command in your VSCode Terminal. Although it's easy to click a button to create a new file, learning these simple commands will be useful in the future.

      code hello_World.py

![Create-new-file](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/VSCode-CreatenewFile.png)

Press Enter, and a new Python file named **hello_world.py** will open in your VSCode. It won't appear in the file tree on the left-hand side of the screen because the file isn't saved yet.

![File-Tree-Example1](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/File-Tree-VSCode.png)

Press `Ctrl + S` to save the newly created Python file, and it will now appear in the file tree.

![File-Tree-Example2](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/File-Tree-VSCode2.png)

You can now start typing your first lines of code in VSCode to print "Hello, World" in your terminal. This type of program is commonly known as a terminal program or application.

Let's start by typing our first line of code:

      print("Hello, World")

![Hello-World-Example1-VS](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Hello-World-VSCode.png)

Once that's done, go to your terminal and type `python` to invoke the Python interpreter. Then, type in the filename `hello_world.py` and press Enter

      python hello_world.py

You should see:

      Hello World

![](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Hello-World-VSCode2.png)

That's how easy it is to write and execute Python code in VSCode. In this tutorial, we've learned how to create a "Hello, World" program in both the terminal interpreter and a text editor. We've also covered creating files and running Python code using the terminal in VSCode.

In the next tutorial, we'll learn about writing comments, their importance, where and why to use them, and how to write them properly.

## Page Navigation

[![Previous Page](https://img.shields.io/badge/Previous%20Page-0077B5?style=for-the-badge)](./b.%20Installing%20Python.md)
[![Next Page](https://img.shields.io/badge/Next%20Page-1DA1F2?style=for-the-badge)](./d.%20Mastering%20Comments.md)
