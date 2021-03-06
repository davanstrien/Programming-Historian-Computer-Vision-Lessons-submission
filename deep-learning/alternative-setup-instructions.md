# Setup 

The main setup instructions can be found on the Programming Historian lesson which this repository accompanies. Although we have done our best to ensure these other options work, we recommend using the Kaggle option unless you have a strong reason not to. 

## Running on another machine 

If you prefer to run the lessons on a local computer or a server you have access to we suggest the following approach to setting up an environment to run the code. Whilst we aim for these instructions to work you will probably have more trouble-free experience by running the code using one of the cloud setup options.

### Required Software 

#### Anaconda 

Anaconda is a Python distribution that provides access to many common Python Data Science packages. Anaconda also has support for virtual environments which allow you to isolate the code used for different projects. If you don't already have Anaconda installed you will need to start by installing the anaconda version for your operating system. If you don't already have anaconda installed we would recommend installing [Minconda](https://docs.conda.io/en/latest/miniconda.html) for Python 3.8. If you already have Conda installed, the full version of Anaconda will also work.  

#### Git

You will need to install [Git](https://git-scm.com/downloads) on your system. If you are running a GNU/Linux or Mac OS operating system it is quite likely you already have Git installed. You can confirm this by running `git --version`. If you have no Git installed see the [install guide](https://github.com/git-guides/install-git) for help getting started. 

### Clone this Github repository

Once you have installed GitHub and Anaconda you should clone this repository using `git clone https://github.com/davanstrien/Programming-Historian-Computer-Vision-Lessons-submission` \ # TODO add final GitGub repo link. 
This command will download the data and notebooks into a new directory inside the directory you are currently working in. 

**!Note** this GitHub repository includes the images used for training the model so it may take a while to clone depending on your network speed. 

### Create a new conda environment 

Once you have cloned the repository change into the newly downloaded directory:

```bash
cd programming-historian-computer-vision-lesson
``` 

This will take you to the main directory for the Programming Historian lesson. Then change into the directory containing the deep learning lessons \# TODO update directory name on publication


```bash
cd deep-learning
```  

Inside this directory run:

```bash
conda env create -f environment.yml
```

This will create a new Conda environment with the required packages installed. If you have issues running this command it might be because you haven't added conda to your `PATH`. Please see the https://docs.anaconda.com/anaconda/user-guide/faq/#installing-anaconda for help. 

```bash
conda activate ph-deep-learning
```

### Start Jupyter 

The Jupyter notebook lessons are inside the directory you should currently be in `deep-learning`. The conda env you have just created contains jupyter lab. To run this you can run

```bash
jupyter notebook
```

This should open up Jupyter lab in your default browser. 

#### Notes for running locally and potential issues
- If you have other conda environments these may register as the default in Jupyter lab. You should be able to change these in the top right of the Jupyter notebook interface when you have a notebook open. Selecting `Python 3` should select the environment you are running the Jupyter notebook from i.e. the one you set up for this lesson. 
- Running code locally may require you to make some changes:
  - depending on your local hardware you might need to reduce to batch size, replace the values following `bs` with a lower value like `8` *should* help with issues related to running out of memory 
  - you may get issues related to multiprocessing. If you get an error which says `RuntimeError: DataLoader worker (pid(s) 95236, 95243, 95245) exited unexpectedly` then you should try turning off multiprocessing. This can be down by adding a new parameter to the `fastai` `dataloaders`: `num_workers=0`
  
