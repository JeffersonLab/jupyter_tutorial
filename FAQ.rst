Tutorial: Using Jupyter at Jefferson Lab
========================================

Frequently Asked Questions about Jupyter at Jefferson Lab
---------------------------------------------------------

Where are my notebooks stored?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For security reasons the jupyter server does not have write access
outside a narrow area. When you log in to jupyter.jlab.org, the file
browser will only show you the files in the directory
``/group/jupyterusers/$USER``. All files outside that directory are only
readable, not writable. You can, however, login to an interactive farm
node and apply version control to the files in
``/group/jupyterusers/$USER``.

How do I use python on interactive farm nodes?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Python is installed on interactive farm nodes at ``/apps/python``. You
can add the python executables to the shell search path automatically at
login by including the following line in your ``.bashrc`` file:

::

    export PATH=/apps/python/3.4.3/bin:$PATH

Instead of the explicit version number you can also specify ``PRO``
which points to python 3.4.3 (as of April 2018).

How do I install a new package?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A selection of commonly used packages are installed system-wide. If a
package you wish to use is not installed system-wide, you can do so
using the interactive farm environment. After adding the python
executables to the shell search path, you will have access to ``pip``
for installing packages in your user base directory ``~/.local``. You
can then install packages using, for example:

::

    pip install --user --upgrade uproot
