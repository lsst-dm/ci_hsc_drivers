==========
``ci_hsc_drivers``
==========

``ci_hsc_drivers`` provides script which exercises the LSST Stack pipe drivers
from single frame through coadd processing based on engineering test data from
Hyper Suprime-Cam provided in the package `ci_hsc`.


Obtaining test data
===================

The data used by ``ci_hsc`` is stored using `Git LFS`_; refer to the `relevant
LSST documentation`_ for details on how to check out this repository.

.. _Git LFS: https://git-lfs.github.com
.. _relevant LSST documentation: http://developer.lsst.io/en/latest/tools/git_lfs.html

Running the tests
=================

Set up the package
------------------

The package must be set up in the usual way before running::

  $ cd ci_hsc_drivers
  $ setup -j -r .


Running the tests
-----------------

Execute ``scons``. On a Mac running OSX 10.11 or greater, you must specify a
Python interpreter followed by a full path to ``scons``::

  $ python $(which scons)

On other systems, simply running ``scons`` should be sufficient.
