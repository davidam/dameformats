
# Table of Contents

1.  [To execute tests:](#org2bd619c)
    1.  [All test](#orgbb6dbb7)
    2.  [Single test's file](#orga244243)
    3.  [Single test](#org9b44860)
2.  [Pypi](#org65e6f1f)


<a id="org2bd619c"></a>

# To execute tests:


<a id="orgbb6dbb7"></a>

## All test

    $ cd dameformats
    $ ./runtests.sh


<a id="orga244243"></a>

## Single test's file

    $ cd dameformats
    $ pytest tests


<a id="org9b44860"></a>

## Single test

    $ cd dameformats
    $ pytest tests/test_damecsv.py::TestDameCsv::test_damecsv_csvcolumn2list 


<a id="org65e6f1f"></a>

# Pypi

-   To install from local:

    $ pip install -e .

-   To install create tar.gz in dist directory:

    $ python3 setup.py register sdist

-   To upload to pypi:

    $ twine upload dist/dameformats-0.1.tar.gz

-   You can install from Internet in a python virtual environment to check:

    $ python3 -m venv /tmp/funny
    $ cd /tmp/funny
    $ source bin/activate
    $ pip3 install dameformats

