tornado-base - a base structure for a tornado app.
===================================================

Not intended for distribution yet, since I haven't yet used it on a real project. Soon :)

## Structure

### config/

A place for your config files. It contains a default config template called
config.default which is versioned. Local installations should use the local_config.py
convenience script to create a local config file which will be ignored by Git. If
any other configuration files are created, and you do not want them to be version, you
have to manually add them to .gitignore.

### handlers/

Your Tornado handlers go in here.

### locale/

Translation csv files.

### log/

Any log files.

### static/

Javascript, CSS, and images go in here.

### templates/

This directory includes both templates and UI modules. The modules are declared in uimodules.py. The base/ subdirectory
can be used for the base template files like base.html (which will be extended by other templates) and error.html.

### tests/

Your unit tests. Includes a run_tests.py file to run all the tests.

### .gitignore

Any stuff you want to ignore from being versioned.

### fabfile.py

If you use Fabric for deplyoment, here's a fabfile for you.

### pip-reqs.txt

Pip requirements. Includes the base requirements for Tornado (tornado 1.2.1 and pycurl 7.19.0).

### urls.py

Your URL patterns.
