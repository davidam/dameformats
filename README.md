
# Table of Contents

1.  [Installing dameformats](#org5662f09)
2.  [Executing tests:](#orgd89d081)
    1.  [All test](#org20308ce)
    2.  [Single test's file](#orgc5cc4d4)
    3.  [Single test](#org7c10c13)
3.  [Making a Pypi package](#org3624990)


<a id="org5662f09"></a>

# Installing dameformats

    $ mkdir venv-dameformats
    $ python3 -m venv venv-dameformats
    $ cd venv-dameformats
    $ source bin/activate
    $ pip3 install dameformats


<a id="orgd89d081"></a>

# Executing tests:


<a id="org20308ce"></a>

## All test

    $ cd dameformats
    $ ./runtests.sh


<a id="orgc5cc4d4"></a>

## Single test's file

    $ cd dameformats
    $ pytest tests


<a id="org7c10c13"></a>

## Single test

    $ cd dameformats
    $ pytest tests/test_damecsv.py::TestDameCsv::test_damecsv_csvcolumn2list 


<a id="org3624990"></a>

# Making a Pypi package

-   To install from local:

    $ pip install -e .

-   To install create tar.gz in dist directory:

    $ python3 -m build

-   To upload to pypi:

    $ twine upload dist/dameformats-0.1.tar.gz

