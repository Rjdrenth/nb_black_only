# nb_black_only

[![PyPI](https://img.shields.io/pypi/v/nb_black.svg)](https://pypi.org/project/nb-black-only/)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nb_black.svg)](https://pypi.org/project/nb-black/)

A simple extension for Jupyter Notebook and Jupyter Lab to beautify Python code automatically using **[Black](https://github.com/psf/black)**.

Please note that the **Black** package only supports Python 3.6+. 
If you edit the code while running the cell, the formatting is
not submitted to the Jupyter notebook and instead silently suppressed, so you have to stick with
the edited, but unformatted code.

Note that this project is a fork of [nb_black](https://github.com/dnanhkhoa/nb_black). This package does not change any functionality, however, support for python versions <3.6 has been disabled and the conditional dependency on yapf (when python is <3.6) has been removed. This has been done to be compatible with [Poetry](https://python-poetry.org/), a great dependency manager for python, which unfortunately did not handle the conditional dependency on yapf properly. This fork will become deprecated if/when Poetry resolves this issue. 

## Installation

You can install this package using [pip](http://www.pip-installer.org):

```
$ [sudo] pip install nb_black_only
```

## Usage

For Jupyter Notebook:

```
%load_ext nb_black
```

For Jupyter Lab:

```
%load_ext lab_black
```

Just put this code into the first cell in your Notebook, and that's all. :)
