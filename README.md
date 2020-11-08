# Introduction to Text-Mining with Python

## Introduction

This repository contains Jupyter notebooks used for teaching the [Cambridge 
Digital Humanities](https://www.cdh.cam.ac.uk) *'Introduction to Text-Mining with Python'*, a series of two 
workshops in the Cambridge Digital Humanities Learning programme 2019.

The notebooks are designed to present material for face-to-face teaching and to 
be a resource for participants to review after the workshops have finished. They 
are also written as stand alone notebooks for anyone to follow and use as they 
wish.

Some of the sections are marked with the words 'going further'. This is 
extension material that we skipped over during the workshops but which is a 
source of deeper exploration into the topics for anyone with further interest 
or more experience.

**Please note that these are the notebooks for the 2019 version of this course. For the 2020 version, please see 
[intro-to-text-mining-with-python-2020](https://github.com/mchesterkadwell/intro-to-text-mining-with-python-2020).**

### Content

The notebooks cover:

*Workshop 1*
* Basic Python (strings, lists, imports, functions, opening/reading files)
* Steps in a text-mining pipeline for research
* Basic text-mining concepts (tokenising, normalising, cleaning, stopwords)
* Creating a frequency distribution and plotting the results

*Workshop 2*
* Introduction to topic modelling (bag-of-words, TF-IDF)
* More basic Python (dictionaries, tuples)
* More basic text-mining concepts (stemming, lemmatization, part-of-speech tagging)
* A basic example of topic modelling using `gensim`
* Visualising topic models with `pyLDAvis`
 
## Code Details

[![Python](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-368/)
[![Python](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-373/)

The aim of the code in this repository is to show basic text-mining techniques 
to participants who are complete beginners to both text mining and coding. 
As such, the notebooks are designed to be run as a teaching aid, not as a 
serious text analysis tool.

The main libraries used in this repository are:
* [Natural Language Toolkit](https://www.nltk.org/) (NLTK)
* [SpaCy](https://spacy.io/) (a bit)
* [Gensim](https://radimrehurek.com/gensim/)
* [pyLDAvis](https://github.com/bmabey/pyLDAvis)
* [Matplotlib](https://matplotlib.org/)

## Quick Start: Launch Notebooks Online

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mchesterkadwell/intro-to-text-mining-with-python/master)

The easiest way to run the Jupyter notebooks in this repository is to click on 
the Binder button above. This will launch a virtual environment in your 
browser where you can open and run the notebooks without installing anything.

## Running Notebooks on Your Own Computer (Beginners)

These instructions are suitable if you have never installed Jupyter Notebooks 
or Python on your own computer before.

### Install Jupyter Notebooks and Python with Anaconda 

[Install Anaconda (Python 3.7)](https://www.anaconda.com/distribution/#download-section). 

Pick the version appropriate for your operating system (Windows, Mac, Linux). 
Make sure you choose ‘Python 3.7’ (not ‘Python 2.7’). 

Once it has installed, [open Anaconda Navigator](http://docs.anaconda.com/anaconda/user-guide/getting-started/#open-navigator).

### Download the Notebooks from GitHub 

Go to the [GitHub page](https://github.com/mchesterkadwell/intro-to-text-mining-with-python ) 
where this code repository is kept. For a simple download, click the ‘Clone or 
download’ green button, then pick 'Download ZIP'.

![](readme-pics/download-or-clone.png)

Open the ZIP file that is downloaded. In most operating systems this will 
 automatically unzip it back into individual files. Move the folder to 
 somewhere you want to keep it, such as 'My Documents'. 

(The more advanced method is to use `git` to clone the repository, but we won’t 
cover that here.)

### Run Notebooks in a Dedicated Environment 

In simple terms, an environment is like an isolated box in which to run a 
notebook safe from interference by other notebooks. Anaconda provides one 
default environment, called ‘root’, in which to get up and running quickly. 
However, you should really make a new environment for each project (which may 
have one or more related notebooks).

In **Anaconda Navigator > Environments** click on the ‘Create’ button in the 
bottom of the Environments list. 

![](readme-pics/create.png)

Type a name e.g. 'intro-to-text-mining', make sure that 'Python' is _checked_ 
and under the dropdown pick '3.7'. Make sure that 'R' is left _unchecked_. 

Then click the ‘Create’ button. 

![](readme-pics/new-env.png)

It will take a few seconds to set up...

Then in **Anaconda Navigator > Environments** make sure you have selected your 
new environment. 

On the right of the environment name is a small green play arrow. Click on it and pick ‘Open Terminal’ from the 
dropdown.

In the Terminal that opens type the following, and press return:

`conda install pip`

![](readme-pics/conda-install-pip.png)

If you do not already have pip installed, it will install it. Otherwise it will give a message:

`# All requested packages already installed.`

Then change directory to wherever you saved the notebooks folder by typing something like:

`cd \path\to\notebooks`

where `path\to\notebooks` is the filepath to wherever you’ve put the notebooks folder.

If you are on a **Mac**, make sure to use forward slashes in the filepath instead e.g. `path/to/notebooks`

![](readme-pics/cd-directory.png)

Then install all the dependencies by typing:

`pip install -r requirements.txt`

This should initiate a big list of downloads and will take a while to finish. Please be patient.

Finally, to launch the Jupyter notebook server type:

`jupyter notebook`

This opens a web page at **http://localhost:8888/tree** showing the project:

![](readme-pics/jupyter-notebooks.png)

If not, you can copy and paste one of the URLs in the Terminal window into your browser e.g. 
http://localhost:8888/?token=ddb27d2a1a6cb29a3483c24d6ff9f7263eb9676f02d71075
(This one will not work on your machine, as the token is unique every time.)

When you are finished with the notebook, press **ctrl+c** to stop the notebook server. 

You can close the Terminal window.

### Starting the Notebook Server Again

Next time you want to start the notebook server:

In **Anaconda Navigator > Environments** make sure you have selected your new environment. 

On the right of the environment name is a small green play arrow. Click on it and pick ‘Open Terminal’ from the 
dropdown.
 To launch the Jupyter notebook server type:

`jupyter notebook`

When you are finished with the notebook, press **ctrl+c** to stop the notebook server. You can close the Terminal window.
