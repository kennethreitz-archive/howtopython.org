The Interpreter
===============

Python is an interpreted language, similiar in the way to how Java operates, with bytecode. However, unlike Java, you will normally work with ``*.py`` files directly, instead of compiled bytecode files (``*.pyc``).

To fire up the Python interpreter, open up your terminal/console application, and type ``python`` or ``python3`` (depending on your installation). You should see something that looks like this::

	Python 3.6.3 (default, Oct  3 2017, 21:45:48)
	[GCC 7.2.0] on linux
	Type "help", "copyright", "credits" or "license" for more information.
	>>>

This is known as the Python interpreter, and is a REPL (Read–Eval–Print Loop). This allows you to type Python code, import modules, and interact with code you've written without having to write files to disk, in an interactive manner. This interactive mode is one of Python's super-powers, compared some other programming lanuages.

Running a Script
----------------

To run a Python script (that you've either written or downloaded from the internet), simply run the following::

    $ python3 name-of-script.py

This will tell Python to load and execute the script provided.

Dependencies
++++++++++++

Sometimes, a script will not run because it does not have the neccessary dependencies installed. You'll normally see this come across as a ``ModuleNotFoundError``, embedded within a confusing (if you're new) exception message::

    Traceback (most recent call last):
      File "name-of-script.py", line 1, in <module>
        import requests
    ModuleNotFoundError: No module named 'requests'

To resolve those dependencies (in this case, ``requests``), ensure you have Pipenv installed (covered in the previous section), and run the following::

    $ pipenv install requests

.. note::

    If you downloaded a directory of files, check for a ``Pipfile`` or a ``requirements.txt`` file in the root directory. If it is present, simply running ``$ pipenv install`` will install all of the dependencies needed, without you needing to specify them.

This will install ``requests`` into a virtual environment. Then, you have two options for running your script:

The first option is to use ``$ pipenv run``::

    $ pipenv run python name-of-script.py

The second option is to run ``$ pipenv shell``, which will spawn a new shell where ``python`` is the one from your virtual environment::

    $ pipenv shell
    (project-vHd3e) $ python name-of-script.py

Note, that if you run ``pipenv shell``, its effects only last during your current terminal session. The next time you load your terminal, you'll have to run ``$ pipenv shell`` again.

Python Interpreter Tricks
-------------------------

``_`` Trick
+++++++++++

The ``_`` variable can be used to reference the last thing that was eval'd (e.g. automatically printed to the screen). For example::

    >>> 1
    1
    >>> a = _
    >>> print(a)
    1

Very useful when using the interactive interpreter!

Bytecode Trick
++++++++++++++

There are a few tricks the interpreter has up its sleeve that I recommend you utilize on a regular basis.

The first trick is ``PYTHONDONTWRITEBYTECODE``. If you set this environment variable (e.g. in your ``~/.bashrc`` file or similar), Python won't write ``*.pyc`` files to disk, which is great, because they are incredibly annoying.

I've been using this environment variable for 7+ years for development and have never had any problems becaue of it.

Interactive Mode Trick
++++++++++++++++++++++

The second trick is to run a Python script, say ``hello.py`` in "interactive" mode, with the ``$ python -i hello.py`` flag.

This flag will run the script, like usual, but will then drop you into a REPL afterwards that has all the locals and globals from the script loaded, for your interactive pleasure. Very useful.
