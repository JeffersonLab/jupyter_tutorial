# Tutorial: Using Jupyter at Jefferson Lab

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/JeffersonLab/jupyter_tutorial/master)
[![Documentation Status](https://readthedocs.org/projects/jupyter-tutorial-at-jefferson-lab/badge/?version=latest)](http://jupyter-tutorial-at-jefferson-lab.readthedocs.io/en/latest/?badge=latest)

This repository contains a self-paced tutorial for using Jupyter, the python notebook interface, for data analysis and visualization at Jefferson Lab.


## Getting Started

The easiest way to get started is to clone this repository to your jupyter.jlab.org workspace by logging in to an interactive farm node over ssh:
- `ssh ifarm`
- `cd /group/jupyterusers/$USER`
- `git clone https://github.com/JeffersonLab/jupyter_tutorial.git`

This will expose the tutorial files to the file browser within jupyter.jlab.org.


## 1. Basic Functionality of Jupyter

* Setting the user base directory and install user packages [(notebook)](1_Basics/setting-python-path.ipynb)
* Reading files and plotting data [(notebook)](1_Basics/read-root-files.ipynb)


## 2. TensorFlow at Jefferson Lab

* Building a 1-D linear regression model of the Qweak asymmetry data [(notebook)](2_TensorFlow/tensorflow-linear-regression-qweak-asymmetries-1dim.ipynb)
* Building a 6-D linear regression model of the Qweak asymmetry data [(notebook)](2_TensorFlow/tensorflow-linear-regression-qweak-asymmetries-6dim.ipynb)


## Frequently Asked Questions about Jupyter at Jefferson Lab

### Where are my notebooks stored?
For security reasons the jupyter server does not have write access outside a narrow area. When you log in to jupyter.jlab.org, the file browser will only show you the files in the directory `/group/jupyterusers/$USER`. All files outside that directory are only readable, not writable. You can, however, login to an interactive farm node and apply version control to the files in `/group/jupyterusers/$USER`.

### How do I use python on interactive farm nodes?
Python is installed on interactive farm nodes at `/apps/python`. You can add the python executables to the shell search path automatically at login by including the following line in your `.bashrc` file:
```
export PATH=/apps/python/3.4.3/bin:$PATH
```
Instead of the explicit version number you can also specify `PRO` which points to python 3.4.3 (as of April 2018).

### How do I install a new package?
A selection of commonly used packages are installed system-wide. If a package you wish to use is not installed system-wide, you can do so using the interactive farm environment. After adding the python executables to the shell search path, you will have access to `pip` for installing packages in your user base directory `~/.local`. You can then install packages using, for example:
```
pip install --user --upgrade uproot
```

## Contributing to this Tutorial

Contributions to this tutorial are welcome. Please fork the repository or create a branch within the organization, develop the tutorial file, and submit a pull-request to merge into the master branch. Pushing into master is restricted to ensure that each tutorial file is reviewed before it is added.

All code contributed to this repository is public, but the code may expect to run on the jupyter.jlab.org system (and may therefore expect to be able to open files in e.g. `/lustre` etc.).

### License

By submitting code to this repository, you are agreeing with the license conditions in LICENSE (Apache License 2.0). Moreover, by submitting code you are asserting that you are in a position to agree to these license conditions (e.g. you are submitting code that is not covered by a more restrictive license).
