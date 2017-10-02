=============================
arccssive2
=============================

arccssive2

.. image:: https://readthedocs.org/projects/arccssive2/badge/?version=latest
  :target: https://readthedocs.org/projects/arccssive2/?badge=latest
.. image:: https://travis-ci.org/coecms/arccssive2.svg?branch=master
  :target: https://travis-ci.org/coecms/arccssive2
.. image:: https://circleci.com/gh/coecms/arccssive2.svg?style=shield
  :target: https://circleci.com/gh/coecms/arccssive2
.. image:: http://codecov.io/github/coecms/arccssive2/coverage.svg?branch=master
  :target: http://codecov.io/github/coecms/arccssive2?branch=master
.. image:: https://landscape.io/github/coecms/arccssive2/master/landscape.svg?style=flat
  :target: https://landscape.io/github/coecms/arccssive2/master
.. image:: https://codeclimate.com/github/coecms/arccssive2/badges/gpa.svg
  :target: https://codeclimate.com/github/coecms/arccssive2
.. image:: https://badge.fury.io/py/arccssive2.svg
  :target: https://pypi.python.org/pypi/arccssive2

.. content-marker-for-sphinx

-------
Install
-------

Conda install::

    conda install -c coecms arccssive2

Pip install (into a virtual environment)::

    pip install arccssive2

---
Use
---

-------
Develop
-------

Development install::

    git checkout https://github.com/coecms/arccssive2
    cd arccssive2
    conda env create -f conda/dev-environment.yml
    source activate arccssive2-dev
    pip install -e '.[dev]'

The `dev-environment.yml` file is for speeding up installs and installing
packages unavailable on pypi, `requirements.txt` is the source of truth for
dependencies.

Run tests::

    py.test

Build documentation::

    python setup.py build_sphinx
    firefox docs/_build/index.html

Upload documentation::

    git subtree push --prefix docs/_build/html/ origin gh-pages