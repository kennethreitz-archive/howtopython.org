Getting Started with Python
===========================

Welcome to Python! Not only are you entering the new world of a programming language, but you are also entering an *ecosystem* of professional and hobbyist developers from literally every corner of the globe coming together to make the world a better place through software (and make a little bit of money at the same time)!

Of course, that last part is optional — you are totally free to code Python on your own and chose not to interact with anyone within the community — but, you'll be missing out on the best part of what makes Python Python!


Twitter Accounts to Follow
--------------------------

Twitter is an excellent way to keep in touch with what's going on with the Python community. Here is a very non–exhaustive (but evolving) list of some suggetions of who to follow on Twitter, to get started:

- **The Python Software Foundation** (`@ThePSF <https://twitter.com/ThePSF>`_)

- **Kenneth Reitz** (`@kennehreitz <https://twitter.com/kennethreitz>`_) — Myself, the author of this website. I often tweet about Python–related topics, as well as music, photography, and other side-projects I have going on.

- **Guido Van Rossum** (`@gvanrossum <https://twitter.com/gvanrossum>`_) — The creator of Python itself. Doesn't tweet much, but is occassionally accessable. Very kind soul. Keep in mind, he gets a lot of attention.

- **Nick Coghlan** (`@ncoghlan_dev <https://twitter.com/ncoghlan_dev>`_) — Core Python developer, very active on Twitter, has very thoughtful thoughts about Open Source and the direction of Python in general.

- **Lynn Root** (`@roguelynn <https://twitter.com/roguelynn>`_) — Closely related to PyLadies.

- **Armin Ronacher** (`@mitsuhiko <https://twitter.com/mitsuhiko>`_) — The creator of Flask, Click, Sphinx, and many other wonderful Python utilities we all know and love. Mostly found writing iOS and Rust code nowadays.

- **Corey Benfield** (`@Lukasaoz <https://twitter.com/Lukasaoz>`_)

- **Alex Gaynor** (`@alex_gaynor <https://twitter.com/alex_gaynor>`_)

- **Yarko T.** (`@yarkot <https://twitter.com/yarkot>`_)

- **David Beazley** (`@dabeaz <https://twitter.com/dabeaz>`_)

- **Brett Cannon** (`@brettsky <https://twitter.com/brettsky>`_)

- **Danny Greenfield** (`@pydanny <https://twitter.com/pydanny>`_)

- **Raymond Hettinger** (`@raymondh <https://twitter.com/raymondh>`_)

- **Jeff Forcier** (`@bitprophet <https://twitter.com/bitprophet>`_) — The creator of Fabric, and maintainer of many open source libraries.

Getting Python Installed
------------------------

Of course, the first thing you need to do is install Python on your machine. If you go to the Python.org website, you may be a bit confused about which version of Python you should be using. *The correct answer is:*

**Use the latest version of Python 3.** As of the time of this writing, that is version **3.7.0**.

Here are some great installation guides for various system types:

- `Installing Python 3 Properly on MacOS <http://docs.python-guide.org/en/latest/starting/install3/osx/>`_
- `Installing Python 3 Properly on Linux <http://docs.python-guide.org/en/latest/starting/install3/linux/>`_
- `Installing Python 3 Properly on Windows <http://docs.python-guide.org/en/latest/starting/install3/win/>`_

Understanding Dependencies
--------------------------

Applications, scripts, and utilities built with Python typically have *dependencies* attached to them, which are Python modules they require to run/operate with, that need to be installed before you can use the software.

A package manager, like *Pipenv* (which we'll cover shortly), or the lower–level *pip* (in conjunction with *virtualenv* can be used to install and manage these dependencies, which are typically hosted on either on `PyPi (The Python Package Index) <https://pypi.python.org/>`_ or `GitHub <https://github.com/>`_.

You'll typically see these required packages (and any specific versions) declared in one of the following files: ``Pipfile``, ``requirements.txt``, or ``setup.py``.

Installing Pipenv
-----------------

The next step is to install *Pipenv*, our packaging tool of choice. Package managers allow us to easily manage (resolve, install, uninstall) dependencies and virtual environments for projects.

Python.org has a `great guide <https://packaging.python.org/tutorials/managing-dependencies/>`_ available for installing Pipenv that also covers its basic usage.

If you're on a Mac, and have `homebrew <https://brew.sh>`_ installed, the following command will suffice::

    $ brew install pipenv

Here's a great `blog post <https://bryson3gps.wordpress.com/2017/11/08/stop-everything-start-using-pipenv/>`_ covering the basic concepts presented by Pipenv, and why it's an excellent choice for your first project.

Using Pipenv
------------

First, ``$ cd`` into your new project directory (after you ``$ mkdir`` and ``$ git init`` it, of course), and simply run ``$ pipenv install requests`` to install the `requests <https://docs.python-requests.org/>`_ library, which is one of our favorites.

Then, run ``$ pipenv shell`` to run a shell that will have a ``$ python`` available in which ``import requests`` will function properly. Pretty simple :)

For further instructions, check out `the Pipenv documentation <https://pipenv.org>`_.

Understanding Source Control
----------------------------

In the Python community, we typically use `git <https://git-scm.org/>`_, a *version control system*. Tools, like git, are used to store all changes to code files, so you can go back to any point in history and reference yourself later if needed. They are also very useful for collaborating with others.

Git is a bit tricky to get started with, but `here's a great guide <https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control>`_ that will get you setup and teach you the basics. It's a requirement if you're ever going to work with Python in a professional environment.
