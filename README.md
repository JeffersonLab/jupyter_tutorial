# Tutorial: Using Jupyter at Jefferson Lab

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/JeffersonLab/jupyter_tutorial/master)

This repository contains a self-paced tutorial for using Jupyter, the python notebook interface, for data analysis and visualization at Jefferson Lab.

## Getting Started

The easiest way to get started is to clone this repository to your jupyter.jlab.org workspace by logging in to an interactive farm node over ssh:
- `ssh ifarm`
- `cd /where/does/this/point`
- `git clone https://github.com/JeffersonLab/jupyter_tutorial.git`

This will expose the tutorial files to the file browser within jupyter.jlab.org.

## 1. Basic Functionality of Jupyter

* Setting the user base directory and install user packages [(notebook)](1_Basics/setting-python-path.ipynb)
* Reading files and plotting data [(notebook)](1_Basics/read-root-files.ipynb)

## 2. TensorFlow at Jefferson Lab

* Building a linear regression model of the Qweak asymmetry data [(notebook)](2_TensorFlow/tensorflow-linear-regression-qweak-asymmetries.ipynb)

## Contributing

Contributions to this tutorial are welcome. Please fork the repository or create a branch within the organization, develop the tutorial file, and submit a pull-request to merge into the master branch. Pushing into master is restricted to ensure that each tutorial file is reviewed before it is added.

All code contributed to this repository is public, but the code may expect to run on the jupyter.jlab.org system (and may therefore expect to be able to open files in e.g. `/lustre` etc.).

### License

By submitting code to this repository, you are agreeing with the license conditions in LICENSE (Apache License 2.0). Moreover, by submitting code you are asserting that you are in a position to agree to these license conditions (e.g. you are submitting code that is not covered by a more restrictive license).
