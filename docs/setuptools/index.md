# Setuptools

## Introduction

What is setuptools? It is a package that is used to create a source distribution and a binary distribution.

## Commands

Installing from `setup.py` is a good idea before publishing to PyPI.

```bash
python setup.py .
```

or cd into the package directory and run the following command:

```bash
pip install .
```

Create a source distribution.

```bash
python setup.py sdist
```

Create a binary distribution.

```bash
python setup.py bdist
```

Create a wheel distribution.

```bash
python setup.py bdist_wheel
```

## Defining a Package with a `setup.py` File

A package is defined in the `setup.py` file. The `setup()` function is used to define the package.

```python
from setuptools import setup

setup(
    name='package_name',
    version='0.0.1',
    description='Package description.',
    long_description='Package long description.',
    author='Author name',
    author_email='Author email',
    url='Package URL',
    packages=['package_name'],
    install_requires=['package_name'],
    classifiers=[
        'Development Status :: 1 - Planning',
        'Intended Audience :: Developers',
        'Programming Language :: Python :: 3',
        'Programming Language :: Python :: 3.6',
        'Programming Language :: Python :: 3.7',
        'Programming Language :: Python :: 3.8',
        'Programming Language :: Python :: 3.9',
        'Programming Language :: Python :: 3 :: Only',
    ],
    python_requires='>=3.6',
)
```

## Defining a Package with a `setup.cfg` File

A package can also be defined in a `setup.cfg` file. The `setup()` function is used to define the package.

## Defining a Package with a `pyproject.toml` File
