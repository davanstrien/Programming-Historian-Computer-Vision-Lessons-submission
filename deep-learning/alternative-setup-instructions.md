# Setup 

The main setup instructions can be found on the Programming Historian lesson which this repository accompanies. Although we have done our best to ensure these other options work, we recommend using the Kaggle option unless you have a strong reason not to. 


## Local setup 

If you prefer to run the lessons on a local computer or a server you have access to we suggest the following approach to setting up the lesson code.

## Required Software 

### Anaconda 

If you don't already have Anaconda installed you will need to start by installing the anaconda version for your operating system. If you don't already have anaconda installed we would recommend installing [Minconda](https://docs.conda.io/en/latest/miniconda.html) for Python 3.8. If you already have Conda installed, the full version of Anaconda will also work. 

### Git
You will need to install [Git](https://git-scm.com/downloads) on your system. If you are running a GNU/Linux operating system it is likely you already have Git installed. You can confirm this by running `git --version`. 


## Clone this Github repository

Once you have installed GitHub and Anaconda you should clone this repository using `git clone url` \ # TODO add final GitGub repo link. 
This command will download the data and notebooks into a new directory inside the directory you are currently working in. 

## Create a new conda environment 

Once you have cloned the repository change into the newly downloaded directory `cd` \ # TODO update directory name 
From this directory run 

`conda create -f environment.yml`

This will create a new Conda environment with the required packages installed. 

`conda activate` \ # TODO confirm conda env name

## Start Jupyter 

`jupyter lab` 


