# CAPL
This is the Git repositiory for the program 'CNN assisted PSF localization (CAPL)' based on the paper Neural Network assisted localization of clustered point spread functions in Single Molecule Localization Microscopy.

## Setting up

The program was developed in Python 3.8.8. Later versions of Python should be supported but have not been tested yet.
If you are on a later version, you may give it a try!

I would suggest you use [Anaconda](https://www.anaconda.com/download/success) / Miniconda and set up a virtual environment as:

- conda create -n "myenv" python=3.8.8 # replace "myenv" with your desired name.

After setting up the virtual environment, you can install the dependencies as:

- pip install -r requirements.txt

- Additionally you will need to set up [Fiji](https://imagej.net/software/fiji/downloads) / ImageJ and install the [ThunderSTORM](https://github.com/zitmen/thunderstorm) plugin.

## Usage

The program is divided into four parts:

1. 01_training_data_generation.ipynb : this notebook generates the training files required to train the model.
2. 02_training_model.ipynb : this notebok trains the CNN model
3. 03_prediction.ipynb : this notebok is used to employ the trained model to predict super-resolved images from unseen data
4. ImageVisualization.py : this script is reused from one of my old projects; used to create the super-resolved image from the detections

A step-by-step procedure for using each notebook is incorporated into the notebooks.

This code is prepared based on [Deep-STORM](https://doi.org/10.1364/OPTICA.5.000458) and [ZeroCostDL4Mic](https://doi.org/10.1038/s41467-021-22518-0) platform. Please also cite their work.

Thank you,

Pranjal Choudhury
