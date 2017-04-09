# UCLA Machine Learning Reading Group: Software Introductions

Getting started with Machine Learning

This README is an introduction to the software that we will use for the reading group. It will be updated as new dependencies are needed.

## git and github

We will distribute code and Juypter notebooks through git and with github. If you are unfamiliar with git, please take this short 10 min. tutorial here:

- https://guides.github.com/activities/hello-world/

## conda environments
We will use conda environments (part of anaconda) in order to isolate the python version and packages that we will be using from interfering with packages you might be using for research. This is especially important given that we will be using python 3.6.

- Introduction to conda: https://conda.io/docs/intro.html
- To install follow instructions here: https://conda.io/docs/install/quick.html
  - The quickest way to install conda is to download the bash script to install miniconda (download the one for python 3.6)
  - Install using ``bash Miniconda3-latest-MacOSX-x86_64.sh
``
  - This should also add some environment variables to your bash startup files. So you need to either restart your terminal or source your bash starup files.
  - Check to see if it works: ``conda list`` to list packages that were installed.
- Once conda is installed, you can create a new environment for the ML reading group
  - ``conda create -n uclaml numpy scipy matplotlib scikit-learn``
  - The previous command creates a new environment named ``uclaml`` that contains four of the packages that we'll need.
- To activate the conda environment, you'll need to use the bash shell
  - ``source activate uclaml``
  - Once in this environment you can install more packages if you forgot to during the initial stage.
    - For example: ``conda install jupyter``  
- To exit the environment:
  - ``source deactivate``

## python and jupyter notebooks
- We will be using python 3.6 for the reading group. This may interfere with your existing code, so we strongly suggest you also use conda.
- We will also use juypter notebook in order to more easily visualize the steps in different machine learning algorithms. Jupyter notebook is similar to mathematica notebooks if you've used those before.
  - A good intro to jupyter notebook is here, which has a web version to try: https://jupyter.readthedocs.io/en/latest/content-quickstart.html
  - Once you've installed jupyter on your computer, you can start the notebook by: ``jupyter notebook``, and it should open a webpage where you can click on jupyter notebook files to open them.
  - Try opening ``test1.ipynb`` in this repository.
