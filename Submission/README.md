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
3. __`LSTM_Model.ipynb`__: Loads the csv data files, either filtered or unfiltered, preprocesses them, compiles the LSTM model and trains it on the training dataset, saves/loads predictions on test dataset, and evaluates and visualises the prediction results. Notebook contains various hyperparameters and directory paths that can be changed manually.
   - The predictions with different parameters of LSTM are also included in `LSTM_Predictions` for evaluation section of the code.

## How to run
To ensure optimal run, it is recommended to run the notebooks in numerical order list in the previous section, and roughly 6-12 hours is recommended. Some of the following conditions are assumed:
- Data are put in `train` and `test` folder, which is in the same location as this notebook.
- GPU is enabled. For CPU run, expect roughly 10 times the recommended time.
- Packages are current up-to-date versions of Google Colab on May 2023 (Python 3.10.11). For list of versions, refer to `package_version.txt`.

### Info specific to __`ResidualCNN_Final.ipynb`__:
- The script was made and ran through Google Colab and the datasets were stored and retrieved from my personal google drive. This drive was mounted to the notebook as seen in the first block of the code. Next, the training and testing features and labels were kept in separately folder. Therefore, when running the code on your end, change the path for 'datas', 'events', 'test_datas' and 'test_events'.
- Ensure you have all the required packages installed and GPU connected. Loading tensorboard again depends on how and where you run the code (this code was written and ran through colab). 
- When compiling the tuned model, ensure that the most optimal hyper-parameters combination is used in case you want to change the hyper-parameters or run the tuning on a different dataset. 
- Finally, there is a block of code in the extra section that visualises the ground truth labels, predicted labels based on a defined threshold and confidence score of a label against time. This is done beyond what was required in the report and hence not included. Furthermore, there is another block of code that shows the Resnet34 model updated to take in 7x7x1 input shape data. Again, this was not used for the purpose of the report.

### Further enquiries  
For enquiries on running the code, the main person in charge of each code part can be contacted:
1. __`Data_Processing_and_Visualisation.ipynb`__: Tuan Khoi Nguyen (tuankhoin@student.unimelb.edu.au)
2. __`ResidualCNN_Final.ipynb`__: Fawad Ahmed Malik (fawadahmedm@student.unimelb.edu.au)
3. __`LSTM_Model.ipynb`__: Sean Breukel (sbreukel@student.unimelb.edu.au),  Victor Bouchet-Hibbert (vbouchet@student.unimelb.edu.au)


