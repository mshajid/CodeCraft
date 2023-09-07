# How to Download and Install Python on Windows

As we went through what and why. In this tutorial, we'll walk you through two methods to install Python on your Windows computer: using the official Python installer and installing it from the Microsoft Store.

## Method A: Installing Python from Official Website

### Step 1: Download Python

1. **Visit Python's Official Website**: Open your web browser and go to the official Python website by clicking [**here**](https://www.python.org/downloads/).

2. **Choose Python 3.x.x (Latest Version)**: On the Python downloads page, you'll find two versions - Python 3.x.x (latest) and Python 2.x (deprecated). We strongly recommend Python 3.x.x for its features, support, and ongoing updates. Click the "Download Python 3.x.x" button.

   **The '3.x.x' in Python 3.x.x represents the specific version number, which can vary over time as Python is updated. For example, it might be '3.9.7' or '3.11.5.' This notation allows you to download the latest available version of Python 3 while disregarding the exact minor and patch version numbers, as they are subject to change with updates.**

   **Note for Beginners**: If you're a beginner, we recommend downloading the latest version from the download page's top section instead of installing any older version. This tutorial will get updated with each major version release, ensuring you have access to the latest information and features.

3. **Select the Installer**: Scroll down the page to find various installation files for different versions and architectures. Most users should choose the 64-bit version. Click on the "Windows installer (64-bit)" link. If you specifically need the 32-bit version, select "Windows installer (32-bit)" instead.

### Step 2: Install Python

4. **Run the Installer**: Once the Python installer is downloaded, locate the installer file in your Downloads folder or the location where you saved it. Double-click the installer file to run it.

5. **Customize Installation (Optional)**: The installer will open a setup window. You have the option to customize the installation by clicking the "Customize installation" button. This allows you to select optional features and customize the installation path. For most users, the default settings are suitable, so you can click "Next" to proceed.

6. **Add Python to PATH (Recommended)**: On the installation window, check the box that says "Add Python X.X to PATH" (where X.X is the Python version number). This option is recommended as it makes it easier to run Python from the command line. Click "Install" to begin the installation.

7. **Installation in Progress**: The installer will start installing Python. You will see a progress bar indicating the installation status.

8. **Installation Complete**: Once the installation is complete, you will see a screen that says "Setup was successful." Congratulations, Python is now installed on your computer!

9. **Verify Python Installation**: To ensure that Python was installed correctly, open a command prompt or terminal window and type the following command:

    ```
    python --version
    ```

    Output on Command Prompt (CMD) or Terminal:
    Python 3.x.x

    If the output is similar to this, then congratulations! You've successfully installed Python on your Windows computer using the official installer.

 If you prefer a visual tutorial, you can watch this video tutorial to learn how to install Python. Please note that the video creator installs Python 3.10, but the installation process is the same across all versions.

[Watch the Video Tutorial](https://youtu.be/2orJ37Swtr4?feature=shared) - How to install Python, a video by Abstract Programmer

## Method B: Installing Python from Microsoft Store

### Step 1: Open Microsoft Store

1. **Launch Microsoft Store**: Press the Windows key on your keyboard or click on the Windows icon in the taskbar to open the Start menu. Type "Microsoft Store" in the search bar and press Enter to launch the Microsoft Store app.

### Step 2: Search for Python

2. **Search for Python**: In the Microsoft Store, use the search bar in the top-right corner and type "Python." Press Enter or click on the search icon.

3. **Select Python**: From the search results, you should see an app named "Python." Click on it to open the Python app page.

### Step 3: Install Python

4. **Install Python**: On the Python app page, you will see an "Install" button. Click on it to begin the installation process.

5. **Installation in Progress**: Microsoft Store will download and install Python on your computer. You will see a progress bar indicating the installation status.

6. **Installation Complete**: Once the installation is complete, you will receive a notification that Python has been successfully installed.

### Step 4: Verify Python Installation

7. **Verify Python Installation**: To ensure that Python was installed correctly, you can open a command prompt or terminal window and type the following command:

    ```
    python --version
    ```

    If the Python version is displayed, such as "Python 3.x.x," then Python has been successfully installed from the Microsoft Store.

Congratulations! You have now installed Python on your Windows computer using the Microsoft Store. You are ready to start using Python for your programming projects.

**If you have any questions or encounter any issues during the installation process, feel free to seek assistance:**

- Join Our Discord Community: We have a vibrant and helpful community on Discord where you can ask questions, share your experiences, and get assistance from fellow Python enthusiasts. Click [here](https://discord.gg/yHXsHjBPw4) to join our Discord server. If you encounter specific errors, please let us know the exact error message, and we will guide you through the troubleshooting process.

- Refer to Python Documentation: The Python documentation is a comprehensive resource that provides detailed information on Python installation and usage. You can find the official Python documentation for Windows [here](https://docs.python.org/3/using/windows.html).

- Search on YouTube: If you encounter any error messages, consider searching on YouTube by typing the exact error message. This can help you find video tutorials addressing your specific issue.

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

### Arch Linux (My Favorite Distro)

1. Open a terminal window and start typing the following command to initiate the download and installation process of Python:

        sudo pacman -S python

2. Once the installation is complete, you can verify it by typing the following command in the same terminal:

        python --version

# Python on Mac OS

If you're using macOS, please follow the installation documentation provided by Python at this link: [Python macOS Installation Documentation](https://docs.python.org/3/using/mac.html).

> **Keep in mind that we are here to help you along the way, so don't hesitate to reach out for any help on discord.**

## Page Navigation

[![Previous Page](https://img.shields.io/badge/Previous%20Page-0077B5?style=for-the-badge)](./a.%20Introduction%20to%20Python.md)
[![Next Page](https://img.shields.io/badge/Next%20Page-1DA1F2?style=for-the-badge)](./c.%20Basic%20Python%20Syntax.md)
