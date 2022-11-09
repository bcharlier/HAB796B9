# Integrated development environment

An Integrated Development Environment (IDE) is a software application that provides comprehensive facilities to computer programmers for software development.
An IDE normally consists of at least a source code editor, build automation tools and a debugger.

## `python`'s specific IDE

There are many IDE for python, but none are perfect, and there is no consensus in the `python` community. There is no real "canonical" choice as `Rstudio` is **the one** for `R` user.

As `python` is a real jackknife programming language, depending on your goal (data scientific program, web development, etc.) you may choose a specific IDE for a particular task.

- Scientific computing : Pyzo, Spyder 
- Generic: PyCharm, VSCode

We warmly recommend you to use an IDE, and we will mostly describe VSCode in what follows.

## VSCode/Codium

For instance you can use `VSCode`. This is a powerful, cross-platform IDE that comes with many extensions.

On the FdS-Linux box, there is a fork of `vscode` called `vscodium`.
You may launch it via the GUI or through the following command line

```bash
$ vscodium
```

### Install a VSCode extension

We will install the `python` extension.
To install it:

1. Open VSCode.
2. Open the Extensions tab (left bar of the VSCode window or simply press `Ctrl+Shift+X`)
3. Type `python` to find the python extension from Microsoft
4. Click the `Install` button, then the `Enable` button

or

1. Open VSCode
2. Press `Ctrl+P` to open the Quick Open dialog
3. Type `ext install ms-python.python` to find the extension
4. Click the `Install` button, then the `Enable` button

or

1. Run in a terminal

```bash
$ vscodium --install-extension ms-python.python
```

----
### <font color='red'>Exercise:</font>

1. Install the `python` extension in your Vscode
----

### An advance text editor

The `keyboard shortcuts Reference guide` is available in the `help` menu (or with `Ctrl+K Ctrl+R` shortcut).
It can be very useful to learn some shortcuts.
For instance:

- Learn how **multicursors** work (e.g., search for an occurrence with `Ctrl+d`)
- Create aligned **multicursors** with `Ctrl+Shift`
- Learn how to move an entire line with `Alt+up`
- etc.

### Using VSCode as a `python` IDE

This part is from the tutorial <https://code.visualstudio.com/docs/python/python-tutorial> to set up `vsCode` to use it as a python IDE. You should have a working `vscode` (with python extension) and `anaconda` program.

----
### <font color='red'>Exercise:</font>

1. Start VS Code in a project (workspace) folder: Using a command prompt or terminal, create an empty folder called `hmma238_test_dir`, navigate into it, and open VS Code (`code`) in that folder (`.`) by entering the following commands:

    ```bash
    cd ~
    mkdir hmma238_test_dir
    cd hello
    code .
    ```
    **Note:** If you're using an Anaconda distribution, be sure to use an Anaconda command prompt.

    By starting VS Code in a folder, that folder becomes your "workspace". VS Code stores settings that are specific to that workspace in `.vscode/settings.json`, which are separate from user settings that are stored globally.

    Alternately, you can run VS Code through the operating system UI, then use `File > Open Folder` to open the project folder.

2. Select a Python interpreter: Python is an interpreted language, and in order to run Python code, you must tell VS Code which interpreter to use. 
    
    From within VS Code, select a Python 3 interpreter by opening the Command Palette (`Ctrl+Shift+P`), start typing the `Python: Select Interpreter` command to search, then select the command. You can also use the `Select Python Environment` option on the Status Bar if available

3. Open the terminal in VS Code and download with `wget` or `curl` the file `test_python.py` at <https://raw.githubusercontent.com/bcharlier/HMMA238/master/Courses/IDE/test_python.py>. Run it through the IDE.


4. Next, you have to learn how to debug a simple `python` script <https://code.visualstudio.com/docs/python/debugging>.

----

## Recommended extensions for VS Code

- Markdown visualizer (extension with TeX rendering even better : [Markdown+Math](https://marketplace.visualstudio.com/items?itemName=goessner.mdmath))
- linter/flake8: [cornflakes](https://marketplace.visualstudio.com/items?itemName=kevinglasson.cornflakes-linter)
- Spell check for less typos: [SpellChecker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
- LaTeX compiler: XXX TODO
- [Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)  to collaboratively edit and debug with others in real time, regardless of your programming language.


