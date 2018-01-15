The Interpreter
===============

Python is an interpreted language, similiar in the way to how Java operates, with bytecode. However, unlike Java, you will normally work with ``*.py`` files directly, instead of compiled bytecode files (``*.pyc``).

To fire up the Python interpreter, open up your terminal/console application, and type ``python`` or ``python3`` (depending on your installation). You should see something that looks like this::

	Python 3.6.3 (default, Oct  3 2017, 21:45:48) 
	[GCC 7.2.0] on linux
	Type "help", "copyright", "credits" or "license" for more information.
	>>> 
	
This is known as the Python interpreter, and is a REPL (Read–Eval–Print Loop). This allows you to type Python code, import modules, and interact with code you've written without having to write files to disk, in an interactive manner. This interactive mode is one of Python's super-powers, compared some other programming lanuages.

Tricks
—————-

Bytecode Trick
//////////////

There are a few tricks the interpreter has up its sleeve that I recommend you utilize on a regular basis. 

The first trick is ``PYTHONDONTWRITEBYTECODE``. If you set this environment variable (e.g. in your ``~/.bashrc`` file or similar), Python won't write ``*.pyc`` files to disk, which is great, because they are incredibly annoying. 

I've been using this environment variable for 7+ years for development and have never had any problems becaue of it.

Interactive Trick
/////////////////

The second trick is to run a Python script, say ``hello.py`` in "interactive" mode, with the ``$ python -i hello.py`` flag. 

This flag will run the script, like usual, but will then drop you into a REPL afterwards that has all the locals and globals from the script loaded, for your interactive pleasure. Very useful. 
