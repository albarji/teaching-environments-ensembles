# Trees and ensembles teaching environment

[![Environment working badge](https://github.com/albarji/teaching-environments-ensembles/actions/workflows/test-environments.yml/badge.svg)](https://github.com/albarji/teaching-environments-ensembles/actions/workflows/test-environments.yml)

Python environment for my Decision Trees and Ensembles lectures.

## Getting started

This environment has been designed for a dedicated **Python 3.14** environment. You have two options for achieving this:

* [conda](https://www.anaconda.com/download) (RECOMMENDED)
* [pyenv](https://github.com/pyenv/pyenv) to install **Python 3.14**, then [virtualenv](https://www.w3schools.com/python/python_virtualenv.asp) to create a dedicated environment.

If you are using Windows I would recommend installing the [Windows Subsystem for Linux](https://learn.microsoft.com/es-es/windows/wsl/install) and following the linux instructions in what follows. If you still prefer installing python natively in Windows, take into account the considerations in what follows.

## A) Using conda

1. Install [Anaconda](https://www.anaconda.com/download) after accepting their terms of service and whatnots.
    * Windows users: make sure you install Anaconda only for your current user, and under a folder that does not contain non-UTF characters (such as **ñ** or **á**).

2. Download the [requirements file](https://raw.githubusercontent.com/albarji/teaching-environments-ensembles/master/requirements.txt) to your computer (right click -> Save link as...).

3. Open a terminal and navigate to the folder where you downloaded the requirements file.
    * Windows users: use an "Anaconda Prompt" instead of the standard Windows terminal.

4. Create a new python environment with

```bash
conda create --name ensembles-labs python==3.14
```

5. Activate the environment

```bash
conda activate ensembles-labs
```

6. Install the requirements

```bash
pip install -r requirements.txt
```

## B) Using pyenv + virtualenv

1. Install [pyenv](https://github.com/pyenv/pyenv?tab=readme-ov-file#installation).
    * Windows users: install [pyenv-win](https://github.com/pyenv-win/pyenv-win) instead. You might need to activate [script execution permissions](https://learn.microsoft.com/es-es/previous-versions/windows/powershell-scripting/hh847748(v=wps.640)?redirectedfrom=MSDN) in your Powershell.

2. Open a terminal and install the required python version.

```bash
pyenv install 3.14
```

3. Download the [requirements file](https://raw.githubusercontent.com/albarji/teaching-environments-ensembles/master/requirements.txt) to your computer (right click -> Save link as...), into the folder where you want to create the virtual environment.

4. Navigate to the folder where you downloaded the requirements file.

5. Activate python version in folder

```bash
pyenv local 3.14
```

6. Create virtual environment

```bash
python -m venv ensembles-labs
```

7. Activate virtual environment

```bash
source ./ensembles-labs/bin/activate
```
* For Windows users: `.\ensembles-labs\Scripts\activate`

8. Install requirements

```bash
pip install -r requirements.txt
