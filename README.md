# Gravitational Lensing Cosmology

This repository contains the hands-on exercise for the "Gravitational Lensing
Cosmology" session of the 19th Heidelberg Summer School (2024) at IMPRS-HD.


## Getting started

To follow along with the hands-on exercise, you will need a number of software
tools.  It is greatly advised to install these in a fresh environment, using
the conda package manager.


## Copying the repository

First, you will need to get a local copy of this repository.  There are two
ways to do so:

If you know the "git" version control system, you can clone this repository.
The URLs can be found under the green "Code" button at the top of this page.

If you are unfamiliar with "git", you can use the green "Code" button at the
top of this page to download a ZIP file that contains the repository.


## Installing mamba or conda

If you do not have an existing mamba or conda installation, you should install
*one* of the following (in that order of preference) using the linked
instructions:

* [miniforge](https://github.com/conda-forge/miniforge) (_preferred_)
* [micromamba](https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html)
* [miniconda](https://docs.anaconda.com/free/miniconda/miniconda-install/)
* [conda](https://docs.conda.io/projects/conda/en/stable/user-guide/install/index.html)

If you do not install the first-choice miniforge distribution, you should
replace all uses of `mamba` below by either `micromamba` or `conda`, as
applicable.


## Setting up the environment

This repository contains a `environment.yml` file that creates an environment
with all necessary software tools for you.

To create the environment, run the following commands inside your local copy of
the repository:

```console
$ mamba env create -f environment.yml
$ conda activate imprs-hd-lensing
$ conda config --env --append channels conda-forge
$ conda config --env --remove channels defaults
```

It is no problem if the last two commands show warnings or errors.

If you ever need to update the environment, you can run the following command:

```console
$ conda deactivate imprs-hd-lensing
$ mamba env update -f environment.yml
$ conda activate imprs-hd-lensing
```


## Running the code

After you have installed all code, you can start running the notebooks for this
exercise.  To do so, launch a Jupyter notebook server from your local copy of
the repository:

```console
$ jupyter notebook
```

This will open a page in your browser from which you can select the individual
exercise notebooks.
