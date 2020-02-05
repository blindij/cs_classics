
# Jupyter Notebooks
## Author: Bjørn Lindi

* *English/Norsk?*
* https://www.coderefinery.org
* Workshop Feb 25-28 at the Technology Library, NTNU

--- 

## From NTNU IT

My group provide High Performance Computing services:
* HPC-systems (idun,Saga, Fram, Betzy). Linux platforms with command line interface and batch systems
* Jupyter Notebooks, primarly for teaching  (Open Stack platform)
* National Storage Infrastructure (NIRD)

---

# Nird Tool kit , https://apps.sigma2.no

<img src="img/nirdtoolkit.png" style="height: 450px;">

--- 

## Anybody who have not install miniconda3 or Anaconda3
https://docs.conda.io/projects/conda/en/latest/user-guide/install/


## Installing Jupyterlab with miniconda3

First we create a separate python environment. We switch to the
environment and start installing packages.
```sh
$ conda create -n jlab-lesson
$ conda activate jlab-lesson
```

Installing packages:
```
(jlab-lesson)$ conda install -c conda-forge jupyterlab
(jlab-lesson)$ conda install nodejs
(jlab-lesson)$ nbdime extensions --enable
(jlab-lesson)$ jupyter labextension install @jupyterlab/git
(jlab-lesson)$ pip install jupyterlab-git
(jlab-lesson)$ jupyter serverextension enable --py jupyterlab_git --sys-prefix
```

---

## Starting Jupyterlab
Make a new subdirectory before you start JupyterLab. We start the
JupyterLab instance with command `jupyter-lab`:
```
(jlab-session)$ mkdir jlab
(jlab-session)$ cd jlab
(jlab-session)$ jupyter-lab
```

## JupyterLab documentation
https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html

## Select Git icon and clone a repository

Here is the GitHub repository to clone:
https://github.com/blindij/cs_classics.git
