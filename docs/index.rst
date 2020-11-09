Plant database
======================================

.. documentation master file.

Nature-Based Solutions (NBS) for river engineering experience incresing popularity to leverage flood risk and ecosystem management in the light of climate change. Even though the demand for NBS is high, there design regarding scale and placement still is an important challenge. In some cases, missing knowledge and trust in NBS leadsto overestimations of costs and time. This plant database constitutes an important step in the design of NBS with a plant data base for river engineering. 


.. This documentation is also as available as style-adapted PDF (`download <https://.readthedocs.io/_/downloads/en/latest/pdf/>`_).

Installation
============

Use ``git`` to download the ``Riverengineering`` repository (make sure to
`install Git Bash`_):

1. Open *Git Bash* (or any other git-able *Terminal*)
2. Create or select a target directory for ``Riverengineering`` (e.g., in your
   *Python* project folder)
3. Type ``cd "D:/Target/Directory/"`` to change to the target
   installation directory.
4. Clone the repository.

.. code:: console

   $ cd "D:/Target/Directory/"
   $ git clone https://github.com/Lukas-create/Riverengineering.git

Now, ``Riverengineering`` lives in ``"D:/Target/Directory/Riverengineering/Riverengineering"``.

Usage
=====

Import
~~~~~~~

1. Run *Python* and add the download directory of ``Riverengineering`` to the
   system path:

.. code:: python

   import os, sys
   sys.path.append("D:/Target/Directory/Riverengineering/")  # Of course: replace "D:/Target/Directory/", e.g., with  r'' + os.path.abspath('')

2. Import ``Riverengineering``:

.. code:: python

   import Riverengineering as 

Example
~~~~~~~

.. code:: python

   import Riverengineering as re
   

Requirements
============

*  Python 3.x (read more on `hydro-informatics.github.io`_)
*  Dependencies:

   * numpy
   * gdal (read more on `hydro-informatics.github.io/geo-pckg <https://hydro-informatics.github.io/geo-pckg.html#gdal>`_)
   * geopandas
   * alphashape
   * shapely


Code Documentation
==================

Package structure
-----------------

.. figure:: https://en.wikipedia.org/wiki/File:UML_diagrams_overview.svg
   :alt: structure



Scripts and functions
---------------------


``Riverengineering`` 
~~~~~~~~~~~~~~~~~~~~~
.. automodule:: plant
   :members:

Search something
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. automodule:: search
   :members:

SQL mgmt
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. automodule:: sqlinput
   :members:


Contributing
=======================

How to document
~~~~~~~~~~~~~~~~

This package uses *Sphinx* `readthedocs <https://readthedocs.org/>`_ and the documentation regenerates automatically after pushing changes to the repositories ``main`` branch.

To set styles, configure or add extensions to the documentation use ``ROOT/.readthedocs.yml`` and ``ROOT/docs/conf.py``.

Functions and classes are automatically parsed for `docstrings <https://www.python.org/dev/peps/pep-0257/>`_ and implemented in the documentation. ``hylas`` docs use `google style <https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html>`_ docstring formats - please familiarize with the style format and strictly apply in all commits.

To modify this documentation file, edit ``ROOT/docs/index.rst`` (uses `reStructuredText <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_ format).

In the class or function docstrings use the following section headers:

For local builds of the documentation, the following packages are required:

.. code:: console

   $ sudo apt-get install build-essential
   $ sudo apt-get install python-dev python-pip python-setuptools
   $ sudo apt-get install libxml2-dev libxslt1-dev zlib1g-dev
   $ apt-cache search libffi
   $ sudo apt-get install -y libffi-dev
   $ sudo apt-get install python3-dev default-libmysqlclient-dev
   $ sudo apt-get install python3-dev
   $ sudo apt-get install redis-server

To generate a local html version of the ``hylas`` documentation, ``cd`` into the  ``docs`` directory  and type:

.. code:: console

   make html

Learn more about *Sphinx* documentation and the automatic generation of *Python* code docs through docstrings in the tutorial provided at `github.com/sschwindt/docs-with-sphinx <https://github.com/sschwindt/docs-with-sphinx>`_


