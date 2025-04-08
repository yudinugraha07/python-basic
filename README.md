# PYTHON BASIC IN PRACTICE

## Overview

This repo is for learning python for beginner.

## Requirements

- Python 3.8 or higher
- pip (Python package installer)
- Virtual environment (optional but recommended)
- Required dependencies listed in `requirements.txt`

## Check Python Installation

To check if Python is already installed on your system, run the following command in your terminal:

```bash
python --version
```

or

```bash
python3 --version
```

If Python is installed, you will see the version number. If not, follow the instructions below to install Python.

## Install Python

1. Visit the [official Python website](https://www.python.org/downloads/).
2. Download the latest version compatible with your operating system.
3. Follow the installation instructions provided for your platform:
    - **Windows**: Run the installer and ensure you check the box to add Python to your PATH.
    - **macOS**: Use the installer or install via Homebrew:
      ```bash
      brew install python
      ```
    - **Linux**: Use your package manager. For example, on Ubuntu:
      ```bash
      sudo apt update
      sudo apt install python3
      ```

## Manage Python Versions

To manage multiple Python versions, you can use a version manager like `pyenv`:

1. Install `pyenv`:
    - **macOS/Linux**:
      ```bash
      curl https://pyenv.run | bash
      ```
    - **Windows**: Use [pyenv-win](https://github.com/pyenv-win/pyenv-win).

2. Add `pyenv` to your shell configuration file (e.g., `.bashrc`, `.zshrc`):
    ```bash
    export PATH="$HOME/.pyenv/bin:$PATH"
    eval "$(pyenv init --path)"
    eval "$(pyenv virtualenv-init -)"
    ```

3. Restart your terminal and install a specific Python version:
    ```bash
    pyenv install 3.10.0
    pyenv global 3.10.0
    ```

4. Verify the installed version:
    ```bash
    python --version
    ```

## Run the App

- Open the terminal
- Go to directory: python-basic
- run the app using this command:
  ```bash
  python app.py
  ```