# Unit Testing in Atom

Once we have written unit tests, you need to be able to run them and check your own code.
Before we start, make sure you have the Atom editor, Python 3, and a GitHub repository already installed in atom.
To check what version of python you are running type `python3 --version` into the terminal (Powershell on Windows). If you have Python 3 or later installed this should print out a version number starting with 3, such as `3.6.3`.

Atom has a quick search feature that can be accessed with the keyshortcut `Shift+Command+P` (for macs) or `Shift+Ctrl+P` (in Windows) or you can manually go to **> Packages > Command Palette > Toggle**.
Search for *settings* and then the *install* subbar. You will need to install the two following atom packages:
`atom-python-test` (from pghilardi)
`atom-python-virtualenv` (also from pghilardi) **Note:** This project says it currently doesn't support Windows or `pip`.

Next, we need to install a virtual enviroment on our machine so that the libraries and python version we have running on this current project won't interfere with our other projects. We can quickly install this using the terminal. Run: `pip3 install pipenv`. `pip3` is a command to install Python3 packages through the terminal rather than going to a website, for example. Use the command `cd` (change directory) and type the location of wherever you have the respository stored, ex. `cd /Users/bob/github/pybasictraining`. Then use the command `pipenv install pytest`.

We need to turn this on in Atom, so go back to the settings page in Atom and go to the packages subbar. Find the `atom-python-virtualenv` package and under its settings, uncheck the first box. Type in the `virtualenv` location, then go under **> Packages > Virtualenv > Select**

You are now done with your installation!

Wherever you have your tests written, with pytest we can now right click on that file.
> pytest

Then click to run all tests.