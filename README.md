# Virtualenv Burrito [![status](http://stillmaintained.com/nogoth/virtualenv-burrito.png)](http://stillmaintained.com/nogoth/virtualenv-burrito) #

With one command, have a working [virtualenv](http://pypi.python.org/pypi/virtualenv) +
[virtualenvwrapper](http://pypi.python.org/pypi/virtualenvwrapper)
environment.

## Install ##

    curl -s https://raw.github.com/nogoth/virtualenv-burrito/master/virtualenv-burrito.sh | bash

## Use

See the
[virtualenvwrapper quickstart](http://www.doughellmann.com/docs/virtualenvwrapper/install.html#quick-start)
or read the
[virtualenvwrapper command reference](http://www.doughellmann.com/docs/virtualenvwrapper/command_ref.html).

### Quickstart ###

To create a new virtualenv:

    mkvirtualenv newname

Once activated, `pip install <package>` (_without_ using sudo) whichever Python
packages you want. They'll only be available in that virtualenv. You can make
as many virtualenvs as you want.

To switch between virtualenvs:

    workon othername

## Upgrade ##

To upgrade to the latest virtualenv + virtualenvwrapper packages:

    virtualenv-burrito upgrade

## Why ##

To get Python coders coding.

Virtualenv Burrito was inspired by
[Pycon sprinters](http://us.pycon.org/2011/sprints/) who wasted time getting
virtualenv setup so they could start hacking on code. It's sadly
complicated to quickly setup the wonderful virtualenv + virtualenvwrapper
environment. Depending on your system you may end up yak shaving with
setuptools, distribute, virtualenv, virtulenvwrapper, .bashrc, PyPI,
apt-get/MacPorts, and more.

A second feature is the ability to upgrade to newer versions of virtualenv and
virtualenvwrapper with a single command.

## Multiple Pythons ##

Both `virtualenv` and `virtualenvwrapper` let you specify which Python interpreter
the virtualenv should use via the `-p` switch. For example:

    mkvirtualenv -p /path/to/some/python coolname

This creates a virtualenv called “coolname” which uses `/path/to/some/python`
as its interpreter. I've tested this with PyPy and it worked great.

## Credits ##

The real hard work is done by the creators of
[Virtualenv](http://www.virtualenv.org/) and
[Virtualenvwrapper](http://www.doughellmann.com/projects/virtualenvwrapper/).
Virtualenv is maintained by [Ian Bicking](ianbicking.org/). Virtualenvwrapper
is maintained by [Doug Hellman](http://www.doughellmann.com/).

## Caveat emptor ##

This simple script is meant for people who do not have virtualenv installed.
