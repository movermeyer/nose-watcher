===============================
Nose-Watcher
===============================

.. image:: https://img.shields.io/pypi/v/nose-watcher.svg
        :target: https://pypi.python.org/pypi/nose-watcher/
        :alt: Latest Version

.. image:: https://img.shields.io/pypi/dm/nose-watcher.svg
        :target: https://pypi.python.org/pypi/nose-watcher

.. image:: https://img.shields.io/pypi/wheel/nose-watcher.svg
        :target: https://pypi.python.org/pypi/nose-watcher/
        :alt: Wheel Status

.. image:: https://travis-ci.org/solarnz/nose-watcher.png?branch=develop
        :target: https://travis-ci.org/solarnz/nose-watcher

.. image:: https://coveralls.io/repos/solarnz/nose-watcher/badge.png?branch=develop
        :target: https://coveralls.io/r/solarnz/nose-watcher?branch=develop

.. image:: https://img.shields.io/pypi/l/nose-watcher.svg
        :target: https://pypi.python.org/pypi/nose-watcher/
        :alt: License


A nose plugin to watch for changes within the local directory.

* Free software: BSD license
* Documentation: http://nose-watcher.readthedocs.org.

Inspired by the `nose-watch <https://github.com/lukaszb/nose-watch>`_ nose
plugin.

Note: nose-watcher will only run on linux, due to the depenency on
`python-inotify` and `inotify`.

Features
--------

* Watches for changes in the local directory, then runs nosetests with the
  specified command line options.

* Doesn't run the tests multiple times if you're using vim, Unlike the similar
  plugin `nose-watch`.

* Specify additional filetypes to watch using the command line argument
  `--filetype`.


Installation
------------

.. code-block:: bash

    pip install nose-watcher

Usage
-----

.. code-block:: bash

    nosetests --with-watcher

    nosetests --with-watcher --filetype .txt

Additional Contributors
-----------------------

*  `Felix Chapman (aelred) <https://github.com/aelred>`_
