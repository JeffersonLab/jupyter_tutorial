Tutorial: Using Jupyter at Jefferson Lab
========================================

|Binder| |Documentation Status|


.. inclusion-marker-0-do-not-remove

This repository contains a self-paced tutorial for using Jupyter, the
python notebook interface, for data analysis and visualization at
Jefferson Lab.


.. inclusion-marker-1-do-not-remove

Getting Started
---------------

The easiest way to get started is to clone this repository to your
jupyter.jlab.org workspace by logging in to an interactive farm node
over ssh:

- ``ssh ifarm``
- ``cd /group/jupyterusers/$USER``
- ``git clone https://github.com/JeffersonLab/jupyter_tutorial.git``

This will expose the tutorial files to the file browser within
`jupyter.jlab.org <https://jupyter.jlab.org>`_.


.. inclusion-marker-2-do-not-remove

Full Documentation
------------------

The complete documentation of this tutorial is avialable at
`Read The Docs <http://jupyter-tutorial-at-jefferson-lab.readthedocs.io/en/latest/>`_.


.. inclusion-marker-3-do-not-remove

1. Basic Functionality of Jupyter
---------------------------------

-  Setting the user base directory and install user packages
   `(notebook) <1_Basics/setting-python-path.ipynb>`__
-  Reading files and plotting data
   `(notebook) <1_Basics/read-root-files.ipynb>`__

2. TensorFlow at Jefferson Lab
------------------------------

-  Building a 1-D linear regression model of the Qweak asymmetry data
   `(notebook) <2_TensorFlow/tensorflow-linear-regression-qweak-asymmetries-1dim.ipynb>`__
-  Building a 6-D linear regression model of the Qweak asymmetry data
   `(notebook) <2_TensorFlow/tensorflow-linear-regression-qweak-asymmetries-6dim.ipynb>`__


.. inclusion-marker-4-do-not-remove

License
~~~~~~~

By submitting code to this repository, you are agreeing with the license
conditions in LICENSE (Apache License 2.0). Moreover, by submitting code
you are asserting that you are in a position to agree to these license
conditions (e.g. you are submitting code that is not covered by a more
restrictive license).

.. |Binder| image:: https://mybinder.org/badge.svg
   :target: https://mybinder.org/v2/gh/JeffersonLab/jupyter_tutorial/master
.. |Documentation Status| image:: https://readthedocs.org/projects/jupyter-tutorial-at-jefferson-lab/badge/?version=latest
   :target: http://jupyter-tutorial-at-jefferson-lab.readthedocs.io/en/latest/?badge=latest
