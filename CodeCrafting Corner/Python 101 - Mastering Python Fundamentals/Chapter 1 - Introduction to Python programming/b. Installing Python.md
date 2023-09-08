# How to Download and Install Python on Windows

There are two simple ways to download and install Python on your Windows computer. You can either use the official installer or get it from the Microsoft Store.

I've outlined the steps for both methods below, so you can choose the one that works best for you and follow the instructions accordingly.


## Method A: How to Install Python Using the Official Installer

### Step 1: Download Python

- **Visit Python's Official Website**: To start, open your web browser and go to the official Python website. You can do this by clicking on this link: [Python Official Website](https://www.python.org/downloads/).
  
- **Choose Python 3.x.x (Latest Version)**: On the Python downloads page, you'll see two options: Python 3.x.x (latest) and Python 2.x (deprecated). For beginners and those new to programming, it's highly recommended to choose Python 3.x.x, which is the latest stable version of Python.

    `Python 3.x.x` represents a specific version of Python. The '`3.x.x`' part might change as new updates are released, but it's always a good idea to pick the latest version because it contains the most up-to-date features, bug fixes, and security improvements.*

    ![Python Download Page](../../../Assets/Python%20Tutorial/Installing%20Python/Python%20Latest%20SS.png)
  
- **Select the Installer**: Scroll down the page to find various installation files for different versions and computer architectures. For most users, the 64-bit version is suitable. So, click on the "Windows installer (64-bit)" link. If you have specific reasons to use the 32-bit version, you can select "Windows installer (32-bit)" instead.

  - *Explanation*: The choice between 64-bit and 32-bit depends on your computer's architecture. Most modern computers use 64-bit architecture, which provides better performance and compatibility with modern software. However, if you have an older computer, you may need the 32-bit version. To check your computer's architecture, you can go to your computer's settings or ask someone knowledgeable about your computer's specifications.

    ![Python Versions Available to Download](../../../Assets/Python%20Tutorial/Installing%20Python/Python%20Versions.png)

By following these simple steps, you'll be on your way to installing Python on your computer, which is the first and crucial step to start programming with Python. Once Python is installed, you'll have access to a powerful and versatile programming language that you can use for various tasks, from simple scripts to complex applications.

### Step 2: Install Python

**Run the Installer** find the downloaded Python installer file in your "Downloads" folder or where you saved it, just like finding a book in your room. Double-click the installer file to begin the installation process, like opening a book to read it.

**5. Customize Installation (Optional)** Sometimes, you might want to customize how Python is installed, like changing the colors of a toy. The installer will show you a window with options, but for most users, the default settings are fine. If you want to keep it simple, click "Next" to continue.

**6. Add Python to PATH (Recommended)** This step is like putting a signpost with Python's name on it so your computer can find it easily. Check the box that says "Add Python X.X to PATH" (where X.X is the Python version number) to make it easier to use Python from the command line. After checking the box, click "Install" to start the installation.

**7. Installation in Progress** Now, the computer will start installing Python, like building a toy. You'll see a progress bar filling up to show the installation status.

**8. Installation Complete** When the installation finishes, you'll see a message saying "Setup was successful." Congratulations! Python is now installed on your computer, like having a new tool to do cool things.

You're all set to start using Python for programming and exciting projects on your computer. Explore and enjoy your programming journey!

### **Verify Python Installation**

To make sure Python was installed correctly, follow these steps:

1. Open a command prompt (Windows) or terminal window (macOS/Linux).

2. Type the following command and press Enter:

    ```shell
    python --version
    ```

3. You should see an output that looks like this:

    ```
    Python 3.x.x
    ```

   If the output is similar to this, congratulations! You've successfully installed Python on your Windows computer using the official installer.

If you prefer a visual tutorial, you can watch this [video tutorial](https://youtu.be/2orJ37Swtr4?feature=shared) to learn how to install Python. Please note that the video creator installs Python 3.10, but the installation process is the same across all versions.

# Installing Python from Microsoft Store on Windows

This tutorial will guide you through installing Python on your Windows computer using the Microsoft Store. This is a beginner-friendly guide.

### Step 1: Open Microsoft Store

1. **Launch Microsoft Store**: Press the Windows key on your keyboard or click the Windows icon in the taskbar to open the Start menu. Type "Microsoft Store" in the search bar and press Enter. This will open the Microsoft Store app.

    ![]()

### Step 2: Search for Python

2. **Search for Python**: Inside the Microsoft Store, you'll find a search bar in the top-right corner. Click it and type "Python." Then, press Enter or click the search icon.

3. **Select Python**: Among the search results, look for an app named "Python." Click on it to open the Python app page.

### Step 3: Install Python

4. **Install Python**: On the Python app page, you'll see an "Install" button. Simply click this button to initiate the installation process.

5. **Installation in Progress**: The Microsoft Store will now download and install Python on your computer. You'll see a progress bar showing the installation status.

6. **Installation Complete**: Once the installation is finished, you'll receive a notification confirming that Python has been successfully installed.

### Step 4: Verify Python Installation

7. **Verify Python Installation**: To ensure Python was installed correctly:

   - a. Open a command prompt or terminal window. You can do this by searching for "Command Prompt" or "Command Prompt" in the Start menu search bar.

   - b. In the command prompt or terminal window, type the following command:

     ```
     python --version
     ```

   - c. Press Enter. If Python was installed correctly, you'll see the Python version displayed, such as "Python 3.x.x."

Congratulations! You've successfully installed Python on your Windows computer using the Microsoft Store. Now, you're ready to begin using Python for your programming projects.

**If you have any questions or encounter issues during the installation process:**

- **Refer to Python Documentation**: The Python documentation is a comprehensive resource that provides detailed information on Python installation and usage. You can find the official Python documentation for Windows [here](https://docs.python.org/3/using/windows.html).

- **Search on YouTube**: If you encounter error messages or need further assistance, consider searching on YouTube using the exact error message. This can lead you to video tutorials addressing your specific issues.

# How to Install Python on Linux

It's important to note that installing Python on Linux follows the same process across all distributions, with the only difference being the package managers that dictate the installation commands.

Some people may choose to change the package managers on their local Linux machines, and they have valid reasons for doing so. However, if you're a beginner, you can stick to the package managers that come pre-installed and follow these steps.

If you're unsure about the Linux distribution you've installed, you can always search for your Linux version. For example, you can use the search term `"I have Arch Linux installed, what is my package manager"`. Odds are, if you have Arch installed, you've already configured your package manager during the OS setup itself. But that's just an Arch joke... you might not get it, hahaha.

### Ubuntu and Debian-based Distros (e.g., Linux Mint)

1. Open the terminal by pressing `Ctrl` + `Alt` + `T` on your keyboard.
2. Now, we're going to update the package lists in your OS by entering the following command in the terminal:

        sudo apt update

    For context, the above terminal command is used on Debian-based distributions to `refresh the local package index`. `It updates a list of package information`, `downloads updated package lists`, and `ensures accurate installation`.

3. Once that is done, you can proceed to install Python using the terminal itself (unlike Windows, you can download Python from the terminal):

        sudo apt install python3

    It is important to include the '`3`' after '`python`,' as omitting it might result in the installation of a previous version of Python (Python 2), which is not recommended due to its end-of-life status.

4. After Python is installed, you can check the installed version in the CLI (which stands for Command Line Interface or the terminal) by typing the following command:

        python3 --version

    This should display the version of Python installed on your computer.

### CentOS and RHEL-Based Distros (e.g., CentOS, RHEL, Fedora)

1. Open your terminal window and enter the following command to start installing Python:

        sudo yum install python3

2. If you're using Fedora, you can use `dnf` instead of `yum`:

        sudo dnf install python3

3. Once the installation is complete, you can verify the installation by typing the following command in the terminal

        python --version

### *Arch Linux (My Favorite Distro)*

1. Open a terminal window and start typing the following command to initiate the download and installation process of Python:

        sudo pacman -S python

2. Once the installation is complete, you can verify it by typing the following command in the same terminal:

        python --version

# How To Install Python on Mac OS

If you're using macOS, please follow the installation documentation provided by Python at this link: [Python macOS Installation Documentation](https://docs.python.org/3/using/mac.html).

> **Keep in mind that we are here to help you along the way, so don't hesitate to reach out for any help on discord.**

## Page Navigation

[![Previous Page](https://img.shields.io/badge/Previous%20Page-0077B5?style=for-the-badge)](./a.%20Introduction%20to%20Python.md)
[![Next Page](https://img.shields.io/badge/Next%20Page-1DA1F2?style=for-the-badge)](./c.%20Writing%20and%20Running%20Python%20Code.md)
