# git-novice

This branch contains the required files to run a JupyterLab-based Binder instance for use by learners participating in the [Supplemental: Using Git from JupyterLab](http://swcarpentry.github.io/git-novice/).

# Running Locally

In order to build the software environments for using Git from Python you will need to have the [Conda](https://docs.conda.io/en/latest/) package management system installed on your machine.

To check whether the Conda is installed on your local machine by running the following command in a terminal.

```bash
$ which conda
```

If Conda has not been installed on your machine, then install the Python 3 version of [Miniconda](https://docs.conda.io/en/latest/miniconda.html) from Anaconda for your OS. Once you have installed Conda on your machine run the following commands in make sure that you have the most recent patches.

```bash
$ conda update -y conda
$ conda init
```

Once Conda has been installed, then you can create and activate the appropriate software environment for the workshop. Python users should run the following commands in the terminal.

```bash
$ cd git-novice
$ git checkout -b binder-python
$ conda env create --prefix ./env --file environment.yml
$ conda activate ./env
```

When you are done you can deactivate the Conda environment by running the following in ther terminal.

```bash
$ conda deactivate
```
