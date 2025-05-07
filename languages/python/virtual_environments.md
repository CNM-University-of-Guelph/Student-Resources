# Virtual Environments

This page introduces the concept of Python virtual environments and why they are important for working on projects that involve external libraries or packages.

A **virtual environment** is a self-contained workspace on your computer where Python and any installed packages exist independently of your system-wide Python installation. This allows you to install, upgrade, and remove packages for a specific project without interfering with other projects or the rest of your system.


## Why Are Virtual Environments Useful?

When working on multiple Python projects, it’s common to use different libraries or library versions. Without virtual environments, all packages would be installed globally, which can lead to:

- Version conflicts between projects
- Accidental upgrades that break existing code
- Difficulty reproducing results or sharing code with others

Virtual environments avoid these issues by creating isolated environments — one per project — so that each project has exactly the packages it needs, and nothing more.


## What Does a Virtual Environment Do?

When you create a virtual environment, Python sets up a dedicated folder that includes:

- A copy of the Python interpreter
- A place to install packages using `pip`
- Scripts and tools for managing the environment

Once the environment is activated, any packages you install or scripts you run will use this local setup instead of your global Python installation.

You can deactivate the environment at any time, returning to your system-wide Python setup.


## How Do You Create a Virtual Environment?

If you're using VS Code or working from the terminal, you'll usually need to create a virtual environment manually. This is a one-time step for each new project.

To create one, open a terminal in your project folder and run:

```bash
python -m venv env
```

This creates a folder named `env` containing the environment. Most IDEs, including VS Code, will automatically detect this environment and allow you to select it as your Python interpreter.

> Note: Some IDEs, like PyCharm, may create virtual environments for you automatically when you start a new project.


## How Do You Activate the Environment?

After creating a virtual environment, you need to **activate it** before installing packages or running your code. This ensures everything stays isolated inside that environment.

### On macOS / Linux:
```bash
source env/bin/activate
```

### On Windows (Command Prompt):
```cmd
env\Scripts\activate
```

Once activated, your terminal prompt will change to show the environment name, like this:

```
(env) your-computer:your-folder user$
```

This indicates you're working *inside* the virtual environment. Now when you run `pip install`, the packages will go into the local `env` directory — not your global Python or Anaconda setup.

If you forget to activate the environment, any packages you install will go to the system-wide Python, which can cause version conflicts or confusion later on.

To deactivate the environment and return to your global setup:
```bash
deactivate
```

## When Should You Use a Virtual Environment?

You should consider using a virtual environment when:

- Starting a new project that will use external packages
- Working on code that depends on specific package versions
- Testing code in a clean, controlled environment
- Avoiding interference with other Python projects

This is a widely adopted practice in Python development and ensures your project is portable, consistent, and isolated from unrelated work.

## Summary

- A virtual environment is an isolated space for Python and its packages.
- It prevents conflicts between projects and keeps your system clean.
- Always activate your virtual environment before installing packages.
- Using environments is a best practice in modern Python development and helps keep your code reproducible and organized.
