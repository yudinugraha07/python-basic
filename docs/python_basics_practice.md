# Python Basics Practice Documentation

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

## Virtual Environment
A virtual environment is a tool that helps to keep dependencies required by different projects in separate places, by creating isolated Python environments for them.

### How to Create a Virtual Environment
1. Run the following command:
   ```bash
   python -m venv env
   ```
2. Activate the virtual environment:
   - On Windows:
     ```bash
     .\env\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source env/bin/activate
     ```

3. To deactivate the virtual environment, simply run:
   ```bash
   deactivate
   ```

## `requirements.txt`
The `requirements.txt` file is used to list all the dependencies of your project. It allows others to install the same dependencies using a single command.

### How to Create `requirements.txt`
1. After installing the required packages in your virtual environment, run:
   ```bash
   pip freeze > requirements.txt
   ```

### How to Install Dependencies from `requirements.txt`
1. Use the following command:
   ```bash
   pip install -r requirements.txt
   ```

## Additional Notes
- Always use a virtual environment to avoid dependency conflicts.
- Keep your `requirements.txt` file updated to ensure reproducibility of your project.