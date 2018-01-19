Text Editors
============

Writing Python code typically involves what it known as a Text Editor. Our recommendation for a text editor is either `Sublime Text 3 <https://www.sublimetext.com/3>`_, which costs money but is free to use, or `Microsoft VS Code <https://code.visualstudio.com>`_.

The functional difference between these two editors is small — they both accomplish the same things, effectively. Which one you chose is a matter of personal taste. There are other editors, like *vim*, *Atom*, or *emacs*, which you may chose to use instead. Whatever works best for you is best.

----------------

I personally use an vastly prefer *Sublime Text 3* to all other options available. It's easily my favorite editor. If it didn't exist though, I'd be using *VS Code*.


.. note::

    Python Requirements for a Text Editor
    -------------------------------------

    There are a few "soft requirements" for a text editor to have, when working professionally (or recreationally), with Python code:

    - Support for "soft tabs"
    - Support for visible whitespace (this is crucial when working with Python files)

    Nice–to–haves:

    - Support for "rulers", which show a horizontal line at line 79, as PEP8 recommends.
    - Built-in linter for showing sytax errors as you type.
    - Built-in support for Flake8, which enforces PEP8 standards as you type.


Sublime Text 3
--------------

.. image:: /_static/sublime.png

Sublime Text doesn't support all of these things by itself, but it comes with a great system called *Package Control*, which allows for easy installation/management of third-party plugins.


Sublime Text 3 Plugin Recommendations
+++++++++++++++++++++++++++++++++++++

- `Package Control <https://packagecontrol.io/installation>`_
    Sublime's Package Manager — can be installed via **
- `Anaconda <https://packagecontrol.io/packages/Anaconda>`_
    Fantastic "Python IDE" for Sublime Text, which offers code linting, PEP8 support, and auto–completion. Works great with Pipenv (and the ``subl`` launcher). Highly recommended.

Additionally Useful Plugins
+++++++++++++++++++++++++++

- `GitSavvy <https://packagecontrol.io/packages/GitSavvy>`_
    Allows you to git push/pull/stage right from Sublime Text.
- `GitGutter <https://packagecontrol.io/packages/GitGutter>`_
    Places the current git status of edited lines in your gutter. Very useful.

Sublime Text 3 Tricks
+++++++++++++++++++++


``subl`` Launcher
/////////////////

Once installed, the command–line ``subl`` launcher will allow you to easily open up projects from your terminal (e.g. ``$ subl .``). In addition, it also will inform plugins like Anaconda of which Python interpreter to use, based on the currently activated virtual environment.

To enable this shortcut, if you're on a Mac, do the following:

    $ ln -s "/Applications/Sublime Text 3.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl

Then, the ``subl`` command will be available to you, always.

PEP8 Rulers
///////////

According to `PEP8 <http://pep8.org/#maximum-line-length>`_, all lines of Python should typically be set to a maximum length of 79 characters (72 if documentation).

Let's configure Sublime Text to display these rulers. Go into *Preferences ➞ Settings*, and add the following JSON::

    "rulers": [
    	72,
    	79,
    ],

Now, you'll see nice horizontal lines at 72 and 79 characters, informing you of how long your lines are!



Microsoft Visual Studio Code (VS Code)
--------------------------------------

.. image:: /_static/vscode.png

Microsoft VS Code guides you through setting up the Python package, built by Microsoft themselves, the first time you run it.

Microsoft VS Code Extensions Recommendations
++++++++++++++++++++++++++++++++++++++++++++

- Python extension for Visual Studio Code
    by Microsoft
    Linting, Debugging (multi-threaded, remote), Intellisense, code formatting, refactoring, unit tests, snippets, Data Science (with Jupyter), PySpark and more.
- vscode-flake8
- MagicPython
    Syntax highlighter for cutting edge Python.

Additionally Helpful Plugins
++++++++++++++++++++++++++++

- Jupyter
    Data Science with Jupyter on Visual Studio Code.
- Django Template
    Django template language support for Visual Studio Code.
- Django Snippets
    Common Django snippets for everyday use.

Microsoft VS Code Tricks
+++++++++++++++++++++

Select a version of Python using *Ctrl + Shift + P*:
    "*Python: Select Interpreter*"

``Microsoft VS Code`` Launcher
/////////////////


Rulers
//////
