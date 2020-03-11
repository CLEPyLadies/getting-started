# getting-started

Basic Python installation instructions and tips

## Installing Python

### Download

Install most recent stable version of Python from [Python.org](https://www.python.org/downloads/).

If you do not already have a favorite text editor or IDE, install the community version of [VS code](https://code.visualstudio.com/download/).

### Verify

From the command line, test if you have python properly installed.
- `python --version` or
- `python3 --version`

Then ensure you have pip
- `pip show pip` or
- `pip3 show pip`

## Python Shell Basics

Open the Python shell (interpreter) from the command line:
- `python` or
- `python3`

Import a built-in library:
- `>>> import this`

This prints _The Zen of Python, by Tim Peters_ below your import statement
(it is technically printing to what is called "stdout"). How neat!
That's really all that the library `this` does, so let's try another library.

Import another built-in library:
- `>>> import antigravity`

Antigravity opens a browser tab with an XKCD comic about exploring Python's rich ecosystem. How cute!

Python has many useful built-in packages, as well.

Import _and do something_ with a useful built-in library:
1. `>>> from datetime import datetime`
1. `>>> that_time = datetime.now()`
1. `>>> datetime.now() - that_time`

The variable `that_time` is storing the timestamp at the moment we entered the command on line 2.
On line 3, we are measuring how much time has passed since creating `that_time`!
Wait a few more seconds and try again:
- `>>> datetime.now() - that_time`

Even more time has passed! The variable `that_time` will store the same timestamp until
we overwrite `that_time` or close the shell.

## Installing Python packages

You use pip to install Python packages that are not in the standard library (not built-in).
- `python -m pip install <<package-name>>`

These are hosted at the Python Package Index, [PyPI](https://pypi.org) ("pie-pee-eye").
Be careful of typos during pip install, as that is one way hackers try to use pip to gain access to your machine.
