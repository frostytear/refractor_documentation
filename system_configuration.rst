====================
System Configuraiton
====================

.. highlight:: console

Dependency Requirements
=======================

The following packages are required to be installed on the target system:

* `CMake <https://cmake.org/>`_ >= 3.2
* `boost <http://www.boost.org/>`_ >= 1.59
* `GNU Scientific Library (GSL) <https://www.gnu.org/software/gsl/>`_ >= 2.0
* `HDF5 <https://support.hdfgroup.org/HDF5/>`_ >= 1.8
* `Python <https://www.python.org/>`_ >= 3.5
* `Lua <https://www.lua.org/>`_ >= 5.2.2 built with a shared library

If a package for Lua that includes a shared library is not available for the target system, a version bundled with the software package can be used. See the :doc:`Compilation <compilation>` instructions for more information.

If you will be modifying the Python bindings, you will additionally need to install:

* `SWIG <http://www.swig.org/>`_ >= 3.0 

`Ruby <https://www.ruby-lang.org/>`_ is also required for some scripts, but not necessary unless you need to run them. We are eventually phasing out the need for Ruby as a requirement.

Python Requirements
===================

The Python bindings to the framework and support Python programs require the following Python packages. Most likely your Linux distribution already has packages available using it's respective package management tool. Otherwise, use the following links for details on installing each package:

* `Numpy/Scipy <http://www.scipy.org/scipylib/download.html>`_
* `Matplotlib <http://matplotlib.sourceforge.net/users/installing.html>`_
* `h5py <http://h5py.alfven.org/docs/guide/build.html>`_
* `PLY (Python Lex-Yacc) <http://www.dabeaz.com/ply/>`_
* `nosetests <http://readthedocs.org/docs/nose/en/latest/>`_

There is a requirements.txt file at the base level of the package that can be used with pip to install the required packages::

    $ pip install -r requirements.txt

Compilers Versions
==================

One of the following combinations of compilers is needed:

* `GCC <https://gcc.gnu.org/>`_ and `GNU Fortran <http://gcc.gnu.org/fortran/>`_ at version 4.6 or greater
* GCC 4.6 or greater and `Intel Fortran Compiler <http://software.intel.com/en-us/intel-compilers/>`_  11.1 or newer

Memory Requirements
===================

Make sure your system has at least 2.5G of memory (including swap) available or else compilation may fail unexpectedly.