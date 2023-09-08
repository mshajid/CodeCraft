# Hello World

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


### Writing "Hello, World" in an IDE (VSCode)

Now that we've tried executing our first lines of code in the terminal, it's time for us to do the same thing in an Integrated Development Environment (IDE). We'll be using VSCode for this.

If you haven't installed VS Code yet, you can follow this tutorial I wrote on how to install it:

| Tutorial Link                                                     | Description                                        |
| ----------------------------------------------------------------- | -------------------------------------------------- |
| [🚀 Click Here](../../../Before%20You%20Start/2.%20Dev-Tools%20Setup%20Guide.md) | Setting Up Development Tools                      |
| [⚙️ Click Here](../../../Before%20You%20Start/3.%20Workspace%20Setup%20Guide.md) | Setting Up Your Workspace in VSCode                |

if you already have VSCode or any other IDEs installed then you can start following the below steps to write an run your code in a text editor.

Open VS Code and Create a new file by typing in this command in your VSCode Terminal, although it is easy to just click a button and create a new file, learning these simple commands will sure come in handy in future.

Type in the following command to in your VSCode Terminal to create a file

      code hello_World.py

![Create-new-file](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/VSCode-CreatenewFile.png)

Press Enter and a new python file named **Hello World.py** will open up on your VSCode but wont show up on the file tree on your left hand side of the screen. that is because the file isnt saved. 

![File-Tree-Example1](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/File-Tree-VSCode.png)

Press `Ctrl + S` to save the newly created python file and it will show up on the file tree.

![File-Tree-Example2](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/File-Tree-VSCode2.png)

Now you can start typing in you first lines of code in VSCode to print Hello World on your terminal. this kind of a program is called terminal programs/applications.

generally in universities or college in first year they tend to teach the basics and they also teach terminal program creations.

to lets start typing in our first line of code 

      print("Hello, World")

![Hello-World-Example1-VS](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Hello-World-VSCode.png)

Once that is done, on your terminal type in `python` to invoke the interpreter and type in the file name `hello_World.py`

      python hello_world.py

and click enter and it should display

      Hello World

![](../../../Assets/Python%20Tutorial/Basic%20Python%20Syntax/Hello-World-VSCode2.png)

that is basically how easy it is to write and execute python codes in VSCode and in this tutorial we learnt how to write `Hello World` program in both Terminal Interpreter and in a text editor and learnt how to create a file and run python codes using terminal in vscode.

in the next tutorial we will learn to write comments and how important it is to write comments and where and why and how to to write it properly.

## Page Navigation

[![Previous Page](https://img.shields.io/badge/Previous%20Page-0077B5?style=for-the-badge)](./b.%20Installing%20Python.md)
[![Next Page](https://img.shields.io/badge/Next%20Page-1DA1F2?style=for-the-badge)](./d.%20Comments.md)
