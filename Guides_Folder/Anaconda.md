# Anaconda package

## Install Anaconda on Ubuntu

Use the command line on terminal (Ctrl + Shift + t):

```bash
sudo apt-get install curl
```

Go with a web browser to "https://repo.anaconda.com/archive" in order to check the latest version (today: Anaconda3-2020.07-Linux-x86_64.sh).

Use the command line on terminal (Ctrl + Shift + t):  
```bash
cd /tmp
curl –O https://repo.anaconda.com/archive/Anaconda3-2020.07-Linux-x86_64.sh
```

Use the command line on terminal (Ctrl + Shift + t):  
```bash
sudo bash Anaconda3-2020.07-Linux-x86_64.sh
```

Follow steps (on dir selection, better to use /home/*user*/anaconda3).

Once finished, activate the installation by entering:  
```bash
source ~/.bashrc
```

Once finished, activate the installation by entering:  
```bash
source ~/.bashrc
```

Use the conda command to test the installation:  
```bash
conda info
```

## Create conda environment

Create a Python 3 environment named test_environment by entering the following:  
```bash
conda create --name test_environment python=3
```
Activate this environment:
```bash
conda activate test_environment
```
## Save a conda environment (.yml)

Activate environment:
```bash
conda activate test_environment
```

Save an environment configuration:
```bash
conda env export > test_environment.yml
```

## Remove a conda environment

```bash
conda remove --name test_environment --all
```

## Creating an environment from an environment.yml file

Create the environment from the environment.yml file:  
```bash
env create -f environment.yml
```

Verify that the new environment was installed correctly:  
```bash
conda env list
```

## List all environments
```bash
conda env list
```

## Rename a environment
```bash
conda create --name new_name --clone old_name
conda remove --name old_name --all # or its alias: `conda env remove --name old_name`
```

## Install Juypiter on a environment
```bash
conda install -c conda-forge jupyterlab
```

## Install jupyter_contrib_nbextensions on a environment

This extensions makes collapasable headings

```bash
conda install -c conda-forge jupyter_contrib_nbextensions
```

## Install pandas on a environment
```bash
conda install pandas
```

## Install xlrd on a environment
```bash
conda install xlrd
```
## Install matplotlib on a environment
```bash
conda install -c conda-forge matplotlib
```
## Install matplotlib on a environment
```bash
conda install -c anaconda seaborn
```
