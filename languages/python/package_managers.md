# Package Managers

When working with programming languages like Python, you’ll often need to install and manage external packages which are reusable pieces of code written by others. A **package manager** is a tool that helps automate this process so you don’t have to download and organize everything manually.

In Python, the most common package managers are `pip` and `conda`. Each serves the same general purpose — installing and managing packages — but they work a bit differently and are used in slightly different contexts.

## Why Use a Package Manager?

Package managers save time and reduce errors by:

- **Automating installs** – You don’t need to find packages online or copy files into your project.
- **Tracking dependencies** – Many packages rely on other packages to work. Package managers install everything you need.
- **Supporting upgrades** – You can easily update packages when new versions are released.
- **Creating reproducibility** – Projects can include a list of required packages (`requirements.txt` or `environment.yml`) so others can recreate the same setup.

Without a package manager, managing project dependencies would be messy and error-prone — especially for larger projects.

## `pip`

`pip` is Python’s built-in package manager. It connects to the Python Package Index (PyPI), a large online collection of open-source packages.

To install a package simply run this command in your terminal:

```bash
pip install pandas
```

To install all the packages listed in a project’s `requirements.txt` file:

```bash
pip install -r requirements.txt
```

`pip` is lightweight and works well for most situations, especially when used inside a virtual environment.

## `conda`

`conda` is both a **package manager** and an **environment manager**. Unlike `pip`, which only install Python packages, `conda` can also install non-Python dependencies like system libraries or compilers which makes it particularly useful in scientific and academic computing.

It also supports creating **virtual environments**, similar to Python's built-in `venv`, so you can manage project-specific dependencies without conflict.

Before using `conda`, you first need to install it by downloading either **Anaconda** or **Miniconda**, which include the `conda` tool. These distributions are especially popular in scientific computing because they simplify the setup process.

To install and get started with `conda`, see the official guide: [Getting started with Conda](https://docs.conda.io/projects/conda/en/stable/user-guide/getting-started.html)

## Choosing Between `pip` and `conda`

Use `pip` if you're using the default Python installation, working inside a virtual environment, or need access to packages from PyPI. `pip` is simple, fast, and works well for most general development needs.

Use `conda` if you're using Anaconda or Miniconda, especially when working with complex packages that require compiled libraries or specific system dependencies. It is also useful for managing both Python and non-Python tools in a unified environment.

In practice, both are widely used. Which one you choose often depends on your setup and the types of packages you need. If you're working with scientific or data-heavy libraries, Anaconda and `conda` are often preferred.

> Avoid mixing `pip` and `conda` in the same environment unless necessary, as it can lead to version conflicts or dependency issues.

## What is Anaconda?

**Anaconda** is a popular Python distribution that comes pre-installed with many scientific and data analysis packages, as well as the `conda` tool. It is widely used in academia and research because it simplifies setup and environment management.

If you're working on a project involving data science or large libraries, Anaconda can be a helpful starting point. It’s especially convenient if you want a complete toolkit without installing each package manually.

To get started with Anaconda:

- Visit the [Anaconda website](https://www.anaconda.com/products/distribution) and download the installer for your operating system.
- Follow the installation instructions provided there.
- After installing, you can open the **Anaconda Navigator** (a graphical interface) or use the terminal with `conda` commands to manage environments and packages.

For a helpful walkthrough, you can also check: [Getting Started with Anaconda](https://docs.anaconda.com/free/anaconda/getting-started/)
