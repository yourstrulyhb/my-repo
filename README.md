# How to setup virtual environment

Hi! This is a document file for creating a virtual environment in Python. Below are the steps and instructions.

## 1. Run `python -m venv <name_of_environment>` in a terminal.

The command above creates a virtual environment. `-m` indicates that we are running a module. Meanwhile, `venv` is the module that creates virtual environment in Python. You may choose any name for your virtual environment but it is common to use `env`.

An example of a terminal to put this command into is the command-line shell or command prompt in Windows.

## 2. Create `.gitignore` file.

Creating a virtual environment installs many scripts, libraries, or dependencies which are heavy to upload. To avoid pushing these files into a remote repository, we can create a `.gitignore` file and include path file patterns that we want `git` to ignore.

We can manually create a `.gitignore` file by creating a new file and labelling it as '.gitignore'.

## 3. Activate virtual environment with correct file.

Inside env\Scripts directory are the activation files to start the virtual environment. Different files are used to activate the virtual environment depending on the terminal used.

For Command Prompt, enter `env\Scripts\activate.bat`.

For Windows Powershell, enter `env\Scripts\Activate.ps1`.

And now your virtual environment is set! Go ahead and keep those programs runnin' (in a safe environment)!

> To deactivate virtual environment, enter `deactivate` command in your terminal.

## 4: Install packages.

After starting your virtual environment, you may want to install useful Python packages for your project or programs.

To do this you may do the following:

### 1. Create `requirements.txt` file.

Create `requirements.txt` file in main directory and input name of packages that you would like to install or include in the virtual environment (e.g. pandas, requests).

### 2. Run `pip install -r requirements.txt`

The command above installs the packages indicated in `requirements.txt`. This will help you install multiple packages in a single command.
