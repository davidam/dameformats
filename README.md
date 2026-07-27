
# Table of Contents

1.  [Installing dameformats](#org002e3dc)
2.  [Executing tests:](#org84285a2)
    1.  [All test](#org8c61579)
    2.  [Single test's file](#orgfdef3f5)
    3.  [Single test](#orgc56729a)
3.  [Making a Pypi package](#orgf4000c5)


<a id="org002e3dc"></a>

# Installing dameformats

    $ mkdir venv-dameformats
    $ python3 -m venv venv-dameformats
    $ cd venv-dameformats
    $ source bin/activate
    $ pip3 install dameformats


<a id="org84285a2"></a>

# Executing tests:


<a id="org8c61579"></a>

## All test

    $ cd dameformats
    $ ./runtests.sh


<a id="orgfdef3f5"></a>

## Single test's file

    $ cd dameformats
    $ pytest tests/test_damecsv.py


<a id="orgc56729a"></a>

## Single test

    $ cd dameformats
    $ pytest tests/test_damecsv.py::TestDameCsv::test_damecsv_csvcolumn2list 


<a id="orgf4000c5"></a>

# Making a Pypi package

-   To install from local:

    $ pip install -e .

-   To install create tar.gz in dist directory:

    $ python3 -m build

-   To upload to pypi:

    $ twine upload dist/dameformats-0.1.tar.gz

