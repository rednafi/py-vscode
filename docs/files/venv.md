# Setting up Environments

## Why Environments are Necessary

The main purpose of using environments is to create a segregation between the dependencies of different python projects. It eliminates (at leas tries to) dependency conflicts since each project has it's own set of dependencies, isolated from one another.

Suppose you are working on two projects, `Project_1` and `Project_2`, both of which have a dependency on the same library, let's say the awesome `Requests` library. Dependency conflict will arise, if for some reason, the two projects need different versions of `Request` library. For example, maybe `Project_1` needs `v1.0.0`, while `Project_2` requires the newer `v2.0.0`.

This can easily be avoided by using individual environment for each project where all the dependencies of the corresponding project will reside. There are multiple ways you can create environment. We'll mainly focus on creating python3 based `conda environment` and native `virtual environment`. Each of them has their own sets of advantages and disadvantages.

## Conda Environments

### Anaconda installation

Install anaconda on your machine. I personally prefer miniconda over the full fledged anaconda.
The installation guide can be found here:

* [Linux](https://docs.anaconda.com/anaconda/install/linux/)
* [MacOS](https://docs.anaconda.com/anaconda/install/mac-os/)

###  Creating Conda Environment
After installing anaconda, to create a python3 environment with a specific version of python, type the following command. This will create an environemnt with python 3.7:

```bash
conda create -n myenv python=3.7
```

### Activating Conda Environment


## Virtual Environment


### Creating Virtual Environments

### Activating Virtual Environments

## Selecting & Switching Environments in VS Code
