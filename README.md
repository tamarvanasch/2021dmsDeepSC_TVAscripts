# 2021dmsDeepSC_TVAscripts
Python scripts from thesis research by Tamar van Asch for the training and evaluation of a CNN using structural brain connectivity data. 

## Introduction

The files in this repository can be used to:

1) Create a DWI based dataset from 2D connectivity matrices
2) Train a classification convolutional neural network (CNN) using this dataset
3) Evaluate the training and predict for a specified test set
4) Apply sensitivity analysis and/or integrated gradients to explain the prediction of the network

An extensive report on this research is added as a pdf file to this repository (0906621_MasterThesis.pdf)

## Organization of files
All the scripts can be found in the folder BrainnetModel_Age. In this folder a serie of files can be found. 
This section aims to briefly state the function or goal of each file.

### 1) Create a DWI based dataset from 2D connectivity matrices
#### Execution files
splitTrainTestCohort.py
createTrain_main.py
createTest_main.py

#### Function files
createInput.py

### 2) Train a classification convolutional neural network (CNN) using this dataset
#### Execution files
brainnet_main.py
brainnetCrossVal_main.py
brainnetEnsemble_main.py

#### Function files
buildModel.py

### 3) Evaluate the training and predict for a specified test set
#### Execution files
crossvalEvaluation_main.py

#### Function files
modelEvaluation.py
 
### 4) Apply sensitivity analysis and/or integrated gradients to explain the prediction of the network
#### Execution files
attrmap_main.py
attrmapIGs_main.py
attrmapIGs_oldVSyoung_main.py

#### Function files
integrated_gradients
process_gradients


## Packages used
The scripts are created in Python (v3.6.8). The CNN is build using Keras (v2.4.2) with Tensorflow (v2.4.1) backend. 
For an overview of all packages used, and the corresponding versions, see the specs.txt file.
