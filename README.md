# Conda Guide
## This guide is a introduction to using Conda, a powerful tool for managing environments and packages. It's a guide for beginners who want to organize data and software development projects efficiently and in isolation.

## Table of Contents
- [Install Conda](#install-conda)
- [Confirm the Installation](#confirm-installation)
- [Create a New Environment](#new-environment)
- [Activate Environment](#activate-environment)
- [Install Libraries](#install-libaries)
- [Run a Script](#run-script)
- [Manage Environments](#manage-environments)

## Install Conda
First, you need to download and execute the installation script for Miniconda, it is a version of the Anaconda distribution.
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```
After the installation, please, reboot your machine.

## Confirm the Installation
Now use the command below to confirm and see the installed packages:
```bash
conda --version
```
To see a list of all packages installed in your base environment:
```bash
conda list
```

## Create a New Environment
Create your first environment with specific Python version and packages isolated from the system:
```bash
conda create -n project-name python=3.10
```
You can list all your environments with:
```bash
conda env list 
```

## Activate Environment
Activate the environment you just created:
```bash
conda activate project-name
```

## Install Libraries
Install libraries inside your active environment. These will only be available within this environment:
```bash
conda install numpy scikit-learn matplotlib
```

To install a specific version of a package, use:
```bash
conda install pandas=2.1.0
```

## Run a Script
To run your code, make sure you are inside your Conda environment, then execute:
(Example)
```bash
python3 my_code.py
```

## Manage Environments

To deactivate the current environment, run:
```bash
conda deactivate
```

To remove an environment:
```bash
conda remove -n project-name --all
```


