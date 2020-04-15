[![Build Status](https://travis-ci.org/neumannd/pytest_fun.svg?branch=master)](https://travis-ci.org/neumannd/pytest_fun)

# Introduction

This GitHub repository is meant for collecting `pytest` example code to introduce colleagues to `pytest`.

# Installation

Get sources from GitHub:

```
$ git clone https://github.com/neumannd/pytest_fun.git
$ cd pytest_fun
```

You can use a [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/) environment with Python 3.8:

```
$ conda create -n pytest_fun python=3.8 pytest numpy
$ conda activate pytest_fun
```

Run the installation:
```
$ python setup.py develop
```

# Run tests

Run all tests with pytest:
```
$ pytest
```

# Examples for projects using pytest

## IOOS Compliance Checker

* url: https://github.com/ioos/compliance-checker
* tests directory: [compliance_checker/tests](https://github.com/ioos/compliance-checker/tree/master/compliance_checker/tests)
* one testing file per module
* pytest decorators: does only use marks
* see `pytest.ini` in root directory for usage of some possible control parameters


# Further Reading

## Using mock modules

Sometimes you have a database or an external service which is not available for your test environment.
In theses cases you can use mock modules to fake the responses of the database/service to return an expected value.
The database/service don't need to be available to run the test code.

* https://docs.pytest.org/en/latest/monkeypatch.html
* https://docs.python.org/dev/library/unittest.mock.html

# Contributors:

* @am-kaiser
* @MacPingu
* @neumannd
