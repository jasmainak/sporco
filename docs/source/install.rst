Installation
============

The simplest way to install the most recent release of SPORCO from
`PyPI <https://pypi.python.org/pypi/sporco/>`_ is

::

    pip install sporco


SPORCO can also be installed from source, either from the development
version from `GitHub <https://github.com/bwohlberg/sporco>`_, or from
a release source package downloaded from `PyPI
<https://pypi.python.org/pypi/sporco/>`_.

To install the development version from `GitHub
<https://github.com/bwohlberg/sporco>`_ do

::

    git clone git://github.com/bwohlberg/sporco.git

followed by

::

   cd sporco
   python setup.py build
   python setup.py install

The install command will usually have to be performed with root
permissions, e.g. on Ubuntu Linux

::

   sudo python setup.py install

The procedure for installing from a source package downloaded from `PyPI
<https://pypi.python.org/pypi/sporco/>`_ is similar.



Requirements
------------

The primary requirements are Python itself, and modules `numpy
<http://www.numpy.org>`_, `scipy <https://www.scipy.org>`_, `future
<http://python-future.org>`_, `pyfftw
<https://hgomersall.github.io/pyFFTW>`_, and `matplotlib
<http://matplotlib.org>`_. Module `numexpr
<https://github.com/pydata/numexpr>`_ is not required, but some
functions will be faster if it is installed. If module `mpldatacursor
<https://github.com/joferkington/mpldatacursor>`_ is installed,
:func:`.plot.plot` will support the data cursor that it provides.

Installation of these requirements is system dependent. Under a recent
version of Ubuntu Linux, the following commands should be sufficient
for Python 2

::

   sudo apt-get install python-numpy python-scipy python-numexpr
   sudo apt-get install python-matplotlib python-pip libfftw3-dev
   sudo pip install future
   sudo pip install pyfftw

or Python 3

::

   sudo apt-get install python3-numpy python3-scipy python3-numexpr
   sudo apt-get install python3-matplotlib python3-pip libfftw3-dev 
   sudo pip3 install future
   sudo pip3 install pyfftw


Some additional dependencies are required for running the unit tests
or building the documentation from the package source. Under a recent
version of Ubuntu Linux, the following commands should be sufficient
for Python 2

::

   sudo apt-get install python-pytest python-numpydoc
   sudo pip install pytest-runner
   sudo pip install sphinxcontrib-bibtex

or Python 3

::

   sudo apt-get install python3-pytest python3-numpydoc
   sudo pip3 install pytest-runner
   sudo pip3 install sphinxcontrib-bibtex
