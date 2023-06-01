# MCEN90048 Assignment 3: EEG Grasp-and-Lift Detection (Code)

**Group 1:**
- Tuan Khoi Nguyen
- Fawad Ahmed Malik
- Sean Breukel
- Victor Bouchet-Hibbert

## Description
This submission consists of all the code needed to replicate the results provided in our Assignment 3 report. This directory consists of the following inputs:
1. __`Data_Processing_and_Visualisation.ipynb`__: Download the dataset, perform data inspection and visualisation, then preprocess them into suitable model inputs. Running this file should return the preprocessed data.
2. __`ResidualCNN_Final.ipynb`__: Loads the 7x7 structured input features along with the labels, preprocesses them, carries out hyper-parameter tuning for the CNN model, display the results, compiles the model with the best combination of hyper-parameters, trains it on training dataset, evaluates it on the test dataset and lastly visualises the results.
3. ...
4. ...

## How to run
To ensure optimal run, it is recommended to run the notebooks in numerical order list in the previous section, and roughly 6-12 hours is recommended. Some of the following conditions are assumed:
- Data are put in `train` and `test` folder, which is in the same location as this notebook
- GPU is enabled. For CPU run, expect roughly 10 times the recommended time
- Packages are current up-to-date versions of Google Colab on May 2023 (Python 3.10.11). For list of versions, refer to `package_version.txt`

For enquiries on running the code, the main person in charge of each code part can be contacted:
1. __`Data_Processing_and_Visualisation.ipynb`__: Tuan Khoi Nguyen (tuankhoin@student.unimelb.edu.au)
2. __`ResidualCNN_Final.ipynb`__: Fawad Ahmed Malik (fawadahmedm@student.unimelb.edu.au)
3. ...: Sean Breukel (...)
4. ...: Victor Bouchet-Hibbert (...)

## Info specific to __`ResidualCNN_Final.ipynb`__:
hjntrmd
