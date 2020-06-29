============
Installation
============

Installation can be done using conda_ or pip_. However, conda is strongly recommended.
Some familiarity with the commandline could come in handy - this is the Terminal in
MacOS and Linux, and the Anaconda Prompt in Windows.

Requirements
============

* Operating system - Animapp has been tested on Windows 10, MacOS High Sierra, and Ubuntu Linux 19.10
* Miniconda3 - A python 3 environment is required, which can be set up using Miniconda (see below)
* Hardware - The OpenCV library is large and takes up a lot of space after installation. The entire Animapp environment needs ~1.5 GB, which should not be difficult in most systems. Other than this, any reasonably modern laptop or home PC should be able to run Animapp.

Install conda
=============

You can skip this section if you already have conda (Anaconda or Miniconda) installed 
on your system. To install conda, go to the Miniconda_ website and install Miniconda3
(python 3) by following the instructions specific to your operating system. Conda can
also be installed with Anaconda_ but this is not required to run Animapp.

Conda channels
==============

Add the ``conda-forge`` channel using ``conda config``::

	conda config --add channels conda-forge


Virtual environment
===================

It is highly recommended that you install Animapp within a virtual environment to ensure that 
all the dependencies are satisfied, and also to keep your python setup organised. 
For example, to create an environment named ``animapp_env``, type the 
following at the commandline::

	conda create -n animapp_env


Install Animapp
===============

First activate the newly created channel::

	conda activate animapp_env
	
Then install the Animapp package::

	conda install -c sraorao animapp

That's it! Check that the installation is working by trying these at the commandline. You 
should see a short message on usage::

	threshold -h
	animapp -h

Operating systems
=================

Animapp has been tested on

* Ubuntu Linux 18.04
* MacOS High Sierra
* Windows 10

.. _conda: https://docs.conda.io/en/latest/
.. _pip: https://pypi.org/project/pip/
.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
.. _Anaconda: https://docs.anaconda.com/anaconda/install/
