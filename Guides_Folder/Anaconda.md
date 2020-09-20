# Anaconda package

## Install Anaconda on Ubuntu

Use the command line on terminal (Ctrl + Shift + t):

`sudo apt-get install curl`

Go with a web browser to "https://repo.anaconda.com/archive" in order to check the latest version (today: Anaconda3-2020.07-Linux-x86_64.sh).

Use the command line on terminal (Ctrl + Shift + t):  
`cd /tmp
curl –O https://repo.anaconda.com/archive/Anaconda3-2020.07-Linux-x86_64.sh`

Use the command line on terminal (Ctrl + Shift + t):  
`sudo bash Anaconda3-2020.07-Linux-x86_64.sh`

Follow steps (on dir selection, better to use /home/*user*/anaconda3).

Once finished, activate the installation by entering:  
`source ~/.bashrc`

Once finished, activate the installation by entering:  
`source ~/.bashrc`

Use the conda command to test the installation:  
`conda info`

## Create conda environment

Create a Python 3 environment named test_environment by entering the following:  
`conda create --name test_environment python=3`

Activate this environment:
`conda activate test_environment`

## Save a conda environment (.yml)

Activate environment:
`conda activate test_environment`

Save an environment configuration:
`conda env export > test_environment.yml`

## Remove a conda environment

`conda remove --name test_environment --all`

## Creating an environment from an environment.yml file

Create the environment from the environment.yml file:  
`env create -f environment.yml`

Verify that the new environment was installed correctly:  
`conda env list`
