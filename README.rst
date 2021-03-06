pct_python_default_test
=======================


Version v0.1.1 as of 2020-08-07 see `Changelog`_

|travis_build| |license| |jupyter| |pypi|

|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|


.. |travis_build| image:: https://img.shields.io/travis/bitranox/pct_python_default_test/master.svg
   :target: https://travis-ci.org/bitranox/pct_python_default_test

.. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
   :target: http://en.wikipedia.org/wiki/MIT_License

.. |jupyter| image:: https://mybinder.org/badge_logo.svg
 :target: https://mybinder.org/v2/gh/bitranox/pct_python_default_test/master?filepath=pct_python_default_test.ipynb

.. for the pypi status link note the dashes, not the underscore !
.. |pypi| image:: https://img.shields.io/pypi/status/pct-python-default-test?label=PyPI%20Package
   :target: https://badge.fury.io/py/pct_python_default_test

.. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/pct_python_default_test
   :target: https://codecov.io/gh/bitranox/pct_python_default_test

.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/pct_python_default_test?branch=master
   :target: https://bettercodehub.com/results/bitranox/pct_python_default_test

.. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/pct_python_default_test?label=CC%20maintainability
   :target: https://codeclimate.com/github/bitranox/pct_python_default_test/maintainability
   :alt: Maintainability

.. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/pct_python_default_test?label=CC%20issues
   :target: https://codeclimate.com/github/bitranox/pct_python_default_test/maintainability
   :alt: Maintainability

.. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/pct_python_default_test?label=CC%20coverage
   :target: https://codeclimate.com/github/bitranox/pct_python_default_test/test_coverage
   :alt: Code Coverage

.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/pct_python_default_test
   :target: https://snyk.io/test/github/bitranox/pct_python_default_test

This is the test project created using PizzaCutter

PizzaCutter is a command-line utility that creates and updates software projects in any language from PizzaCutter project templates.

The purpose of this repository is, to show and test a newly created project from the python default template.


More Information can be found here :
    - `PizzaCutter <https://github.com/bitranox/PizzaCutter>`_
    - `PizzaCutter python default template <https://github.com/bitranox/pct_python_default>`_
    - more templates to come

----

automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
.com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)

Python version required: 3.6.0 or newer

tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.8-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64

`100% code coverage <https://codecov.io/gh/bitranox/pct_python_default_test>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/pct_python_default_test>`_, automatic daily builds and monitoring

----

- `Try it Online`_
- `Usage`_
- `Usage from Commandline`_
- `Installation and Upgrade`_
- `Requirements`_
- `Acknowledgements`_
- `Contribute`_
- `Report Issues <https://github.com/bitranox/pct_python_default_test/blob/master/ISSUE_TEMPLATE.md>`_
- `Pull Request <https://github.com/bitranox/pct_python_default_test/blob/master/PULL_REQUEST_TEMPLATE.md>`_
- `Code of Conduct <https://github.com/bitranox/pct_python_default_test/blob/master/CODE_OF_CONDUCT.md>`_
- `License`_
- `Changelog`_

----

Try it Online
-------------

You might try it right away in Jupyter Notebook by using the "launch binder" badge, or click `here <https://mybinder.org/v2/gh/{{rst_include.
repository_slug}}/master?filepath=pct_python_default_test.ipynb>`_

Usage
-----------

- example for including docstrings

.. code-block:: python

    def main() -> None:
        """
        the main method, prints hello world


        Parameter
        ----------
        none
            none


        Result
        ----------
        none


        Exceptions
        ----------
        none


        Examples
        ----------

        >>> main()
        Hello World - by PizzaCutter

        """

Usage from Commandline
------------------------

.. code-block:: bash

   Usage: pct_python_default_test [OPTIONS] COMMAND [ARGS]...

     a pizzacutter default test project, crated with PizzaCutter and the
     PizzaCutter default python template

   Options:
     --version                     Show the version and exit.
     --traceback / --no-traceback  return traceback information on cli
     -h, --help                    Show this message and exit.

   Commands:
     info  get program informations

Installation and Upgrade
------------------------

- Before You start, its highly recommended to update pip and setup tools:


.. code-block:: bash

    python -m pip --upgrade pip
    python -m pip --upgrade setuptools
    python -m pip --upgrade wheel

- to install the latest release from PyPi via pip (recommended):

.. code-block:: bash

    # install latest release from PyPi
    python -m pip install --upgrade pct_python_default_test

    # test latest release from PyPi without installing (can be skipped)
    python -m pip install pct_python_default_test --install-option test

- to install the latest development version from github via pip:


.. code-block:: bash

    # normal install
    python -m pip install --upgrade git+https://github.com/bitranox/pct_python_default_test.git

    # to test without installing (can be skipped)
    python -m pip install git+https://github.com/bitranox/pct_python_default_test.git --install-option test

    # to install and upgrade all dependencies regardless of version number
    python -m pip install --upgrade git+https://github.com/bitranox/pct_python_default_test.git --upgrade-strategy eager


- include it into Your requirements.txt:

.. code-block:: bash

    # Insert following line in Your requirements.txt:
    # for the latest Release on pypi:
    pct_python_default_test

    # for the latest development version :
    pct_python_default_test @ git+https://github.com/bitranox/pct_python_default_test.git

    # to install and upgrade all modules mentioned in requirements.txt:
    python -m pip install --upgrade -r /<path>/requirements.txt



- to install the latest development version from source code:

.. code-block:: bash

    # cd ~
    $ git clone https://github.com/bitranox/pct_python_default_test.git
    $ cd pct_python_default_test

    # to test without installing (can be skipped)
    python setup.py test

    # normal install
    python setup.py install

- via makefile:
  makefiles are a very convenient way to install. Here we can do much more,
  like installing virtual environments, clean caches and so on.

.. code-block:: shell

    # from Your shell's homedirectory:
    $ git clone https://github.com/bitranox/pct_python_default_test.git
    $ cd pct_python_default_test

    # to run the tests:
    $ make test

    # to install the package
    $ make install

    # to clean the package
    $ make clean

    # uninstall the package
    $ make uninstall

Requirements
------------
following modules will be automatically installed :

.. code-block:: bash

    ## Project Requirements
    click
    cli_exit_tools @ git+https://github.com/bitranox/cli_exit_tools.git

Acknowledgements
----------------

- special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"

Contribute
----------

I would love for you to fork and send me pull request for this project.
- `please Contribute <https://github.com/bitranox/pct_python_default_test/blob/master/CONTRIBUTING.md>`_

License
-------

This software is licensed under the `MIT license <http://en.wikipedia.org/wiki/MIT_License>`_

---

Changelog
---------

- new MAJOR version for incompatible API changes,
- new MINOR version for added functionality in a backwards compatible manner
- new PATCH version for backwards compatible bug fixes

v0.1.1
---------
2020-08-01: fix pypi deploy

v0.1.0
--------
2020-07-31:
    - change1
    - change2
    - ...

