Python
=======

Summary
--------
 1. Use [PEP 8](http://www.python.org/dev/peps/pep-0008/) and [validate](https://pypi.python.org/pypi/pep8) style.
 2. Use virtual-env and pip. Include both in repositories.
 

Managing Dependencies
----------------------

When starting a new project, do the following:

    $ virtualenv ENV
    $ . ENV/bin/activate
    $ touch requirements.txt

Add dependencies to [requirements.txt](http://www.pip-installer.org/en/latest/requirements.html), then run:

    $ pip install -r requirements.txt
    $ git add ENV requirements.txt
    $ git commit