# Teaching Environments

|Linux|Mac OS X|Windows|
|-----|--------|-------|
|[![Build Status](https://travis-ci.org/albarji/teaching-environments-ensembles.svg?branch=master)](https://travis-ci.org/albarji/teaching-environments-ensembles)|[![Build Status](https://travis-ci.org/albarji/teaching-environments-ensembles.svg?branch=master)](https://travis-ci.org/albarji/teaching-environments-ensembles)|[![Build status](https://ci.appveyor.com/api/projects/status/jb3rcrh3n0pavv5c?svg=true)](https://ci.appveyor.com/project/albarji/teaching-environments-ensembles)|

Conda environments for Decision Trees and Ensembles lectures.

## Usage

First install a **Python 3, 64-bits** [Conda distribution](https://anaconda.org/anaconda/python). If you are using Windows make sure you install Anaconda only for your current user, and under a folder that does not contain non-UTF characters (such as **ñ** or **á**). After installing follow the instructions for your particular operative system.

## Linux or Mac

Download the [environment file](https://raw.githubusercontent.com/albarji/teaching-environments-ensembles/master/environment.yml) to your computer (right click -> Save link as...) and open a terminal in the same folder. Then type

    conda env create -f environment.yml

to create an environment named `ensembles-labs` with the necessary packages.

After creating the environment, open a terminal in the folder with the notebooks you want to work with. Then log into the environment running

    source activate ensembles-labs

and then type

    jupyter notebook

to start the notebook server.

## Windows

Download the [environment file](https://raw.githubusercontent.com/albarji/teaching-environments-ensembles/master/ensembles/environment.yml) to your computer (right click -> Save link as...) and open an **Anaconda Navigator**. Click on the **Environments** tab, and look for the **Import** button. After clicking it, select as **Specification file** the environment file you downloaded. This will create an environment named `ensembles-labs` with the necessary packages. Note the creation process might take a while.

After creating the environment, click the play icon at the environment name, and choose the option to launch a Jupyter notebook.

If for whatever reason the Jupyter notebook launch fails, you can also try opening an Anaconda Prompt in the folder with the notebooks you want to work with, then log into the environment running

    activate ensembles-labs

and then type

    jupyter notebook

to start the notebook server.
