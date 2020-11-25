# TDT4173-project

## Overview:

- fpl_data.csv is the dataset to build the models.
- Data.ipynb fetches and preprocesses the data and then saves the data in the file called fpl_data.csv.
- Models.ipynb defines and builds the models based on fpl_data.csv, as well as evaluating and comparing the models.


## Setup:

1. Clone repo and cd into folder: `git clone https://github.com/Markusmk101/TDT4173-project.git` and `cd TDT4173-project`
2. Install requirements: `pip install -r requirements.txt`
3. Open notebook: `jupyter notebook`

## Run code:

#### If you want to run the data preprocessing:
1. Delete the file fpl_data.csv.
2. Open Data.ipynb an click on "run all cells". Then the outputs can be viewed beneath each cell. This will create a new file called fpl_data.csv. Make sure this is placed in the same directory as the Models.ipynb file.
   - NOTE: This file takes some time to run. Approximately **1 hour** on a personal computer. You can skip this step. 
   - Ignore the warnings.

#### Or skip directly to the model training, as we have already uploaded fpl_data.csv to save you the time:
1. Open Models.ipynb and click on "run all cells". Then the outputs can be viewed beneath each cell.
   - NOTE: When running this file, a folder called logs will be created in the same folder as this file. This is logs used by tensorboard. If you decide to run the notebook several times, make sure to delete the logs folder before each run. 



##### Both of the ipynb files shold be sufficent commented for you to follow the code.
