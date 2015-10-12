# Python Autocomplete Package [![Build Status](https://travis-ci.org/sadovnychyi/autocomplete-python.svg)](https://travis-ci.org/sadovnychyi/autocomplete-python)

Python variables, methods, functions and modules autocompletions in Atom.

This is powered by [Jedi](https://github.com/davidhalter/jedi).

![Demo](https://cloud.githubusercontent.com/assets/193864/7394244/e6906980-eec4-11e4-9ee2-8749d16ff468.gif)

# Features

* Works on all platforms: :apple: Mac OS, :penguin: Linux and :checkered_flag: Windows
* Works with both :snake: Python 2 and 3
* Watches whole package of the file you're currently editing
* Configurable additional PATHs to include for completions (global for now)
* You can include project specific folders by using $PROJECT variable in PATH configuration
* Highlights UPPERCASE_VARIABLES as constants according to PEP8
* Highlights builtin functions and variables with special style
* Prints first N characters of statement value while completing variables
* Prints function arguments while completing functions
* Go-to-definition functionality, by default on `Ctrl+Cmd+G`/`Ctrl+Alt+G` (thanks to [@patrys](https://github.com/patrys))

# Installation

* Be sure to use Atom 0.199 or newer
* Install [autocomplete-python](https://github.com/sadovnychyi/autocomplete-python).
* If using a [virtualenv](https://virtualenv.pypa.io/en/latest/) with third-party packages, be sure to launch Atom from the [activated virtualenv](https://virtualenv.pypa.io/en/latest/userguide.html#activate-script) to get completion for your third-party packages!
* If you're on Windows:
  * Install [python](https://www.python.org/downloads/).
  * Make Sure that python is available in your PATH: `echo %PATH%`. If it's not, add it and restart your system: `set PATH=%PATH%;C:\Python27`
* Be sure to check package settings and adjust them. Please read them carefully before creating any new issues.
  * Set path to python directory if package cannot find your python executable
  * Set extra path if package cannot autocomplete external python libraries
  * Select one of autocomplete function parameters if you want function arguments to be completed
  * Note that add bracket after function and add dot after module does not works properly
![image](https://cloud.githubusercontent.com/assets/193864/10421412/d6e02974-70da-11e5-81c9-a77d0c80896b.png)


# Common problems

* "Error: spawn UNKNOWN" on Windows.
  * Solution: Find your python executable and uncheck the "Run this program as an administrator". See issue [#22](https://github.com/sadovnychyi/autocomplete-python/issues/22).

