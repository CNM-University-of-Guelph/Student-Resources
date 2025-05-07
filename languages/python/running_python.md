# Running Python

This page will guide you through running Python code on your system. Once Python is installed, the next step is learning how to execute Python programs. There are two main ways to do this: using a code editor like Visual Studio Code (VS Code), or using the command line (Terminal or Command Prompt).

Both approaches achieve the same result — running `.py` files — but offer different experiences. VS Code provides a beginner-friendly interface with helpful features like syntax highlighting and autocompletion, while the command line gives you a lightweight, direct way to interact with your system and scripts.

Ultimately, both methods are worth learning. It’s common to use VS Code for writing and editing code, but still rely on the terminal to run, test, or debug certain parts.

## Option 1: Running Python in Visual Studio Code

Visual Studio Code is a free, cross-platform code editor that supports Python with extensions. If you haven’t installed it yet, follow this guide: [Installing VS Code](../../ide/vscode_install.md)

### Why use VS Code?

VS Code offers many beginner-friendly features:
- You can easily open files and folders
- It highlights errors and gives hints as you write
- It lets you run scripts with a single click (after a one-time setup)

Once VS Code is installed, follow these steps to prepare it for running Python code:

### 1. Install the Python Extension

VS Code does not come with Python support by default. You need to install the extension:
- Open VS Code
- Go to the Extensions tab (left sidebar, or press `Ctrl+Shift+X` / `Cmd+Shift+X`)
- Search for **"Python"** by Microsoft and click **Install**

This extension enables syntax highlighting, code linting, and easy script execution.

### 2. Select a Python Interpreter

VS Code can detect multiple Python versions on your machine. You need to tell it which one to use:
- Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS) to open the Command Palette
- Search for and select **Python: Select Interpreter**
- Pick the interpreter for Python 3.10 or higher

If no interpreters are found, make sure Python is installed and added to your system’s PATH.

### 3. Create Your Project Folder and Script

You’ll need a folder to keep your files organized:

- In VS Code, go to **File > Open Folder...**
- Create a new folder (e.g., `python-test`) and open it
- Inside the folder, create a new file and save it as `hello.py`

This is where you’ll write and run your first Python script.

### 4. Write and Run Your First Script

In `hello.py`, add the following line:

```python
print("Hello, world!")
```

Now, look for the ▶️ **Run Code** button in the top-right corner of the window and click it. This will run your script using the interpreter you selected earlier.

### 5. Check the Output

If everything is working correctly, the **Terminal** panel at the bottom of the window should show:

```
Hello, world!
```

If you see an error or the button isn’t visible, double-check that:
- The Python extension is installed
- The interpreter is selected
- You saved your file as a `.py` file (not `.txt`)


## Option 2: Running Python from the Command Line

If you prefer using the command line (or want to understand what’s happening behind the scenes), you can run Python scripts directly from Terminal or Command Prompt.

### Why use the command line?

- It’s lightweight and doesn’t require an editor
- You can quickly test or rerun scripts
- It’s how many servers and data processing tools operate

### macOS / Linux Instructions

1. Open Terminal.
2. Navigate to the folder where your script is saved:
   ```bash
   cd /path/to/your/folder
   ```
3. Create a file called `hello.py` (you can use a code editor or run `nano hello.py`) and type:
   ```python
   print("Hello, world!")
   ```
4. Save the file, then run:
   ```bash
   python3 hello.py
   ```

You should see:

```
Hello, world!
```

### Windows Instructions

1. Open Command Prompt.
2. Use the `cd` command to go to your script’s folder:
   ```cmd
   cd path\to\your\folder
   ```
3. Create a new file called `hello.py` using Notepad or your editor, and add:
   ```python
   print("Hello, world!")
   ```
4. Run the script:
   ```cmd
   python hello.py
   ```

If Python is installed and configured correctly, you’ll see:

```
Hello, world!
```

If not, you may need to use `python3` or check your PATH variable.


## Re-running Your Script

Once your script is written, you’ll likely want to run it multiple times while making changes.

- In **VS Code**: Just save the file and click the **Run** button again
- In **Terminal**: Press the ↑ arrow key to repeat the last command, then press **Enter**

This lets you test changes quickly and avoid retyping commands.
