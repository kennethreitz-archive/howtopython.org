The Interpreter
===============



Tricks
—————-

Bytecode Trick
//////////////

There are a few tricks the interpreter has up its sleeve that I recommend you utilize on a regular basis. 

The first trick is ``PYTHONDONTWRITEBYECODE``. If you set this environment variable (e.g. in your ``~/.bashrc`` file or similar), Python won't write ``*.pyc`` files to disk, which is great, because they are incredibly annoying. 

I've been using this environment variable for 7+ years for development and have never had any problems becaue of it.

Interactive Trick
/////////////////

The second trick is to run a Python script, say ``hello.py`` in "interactive" mode, with the ``$ python -i hello.py`` flag. 

This flag will run the script, like usual, but will then drop you into a REPL afterwards that has all the locals and globals from the script loaded, for your interactive pleasure. Very useful. 