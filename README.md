# DSDN Starbucks Capstone Project

Capstone project for Data Scientist Nanodegree Program of Udacity

### Table of Contents

1. [Installation](#installation)
2. [Project description](#objective)
3. [File descriptions](#files)
4. [Results](#results)
5. [Acknowledgements](#final)


## Installation <a name="installation"></a>
For running the notebook with analysis, a version of python > 3.8, is needed.
There aren't more python library needed than the ones with anaconda.

## Project description <a name="objective"></a>
The objective of the project is to analyse a dataset given by Starbucks, with promotional offer sent to user, and purchases made by them.
The dataset is not made by real data, but simulated ones.
The purpose is to clean the dataset, analyze it, and prepare a sort of raccomandation engine to select which offer sent to which users, in order to maximize the impact.

## File descriptions <a name="files"></a>

### Dataset
The dataset is in the made of three files, stored in the `/data` folder:
- `portfolio.json` - containing offer ids and meta data about each offer (duration, type, etc.)
- `profile.json` - demographic data for each customer
- `transcript.json` - records for transactions, offers received, offers viewed, and offers completed
A better explanation of the files structure is in the notebook

### Other files
All analysis are in the `Starbucks_Capstone_notebook.ipynb` notebook; 
There is a description of the project and data, and the main steps of the analysis are:
- Load data & inspection
- Data cleaning
- Statistical analysis
- ML classification & tuning
- ML regression (only a test)


## Results<a name="results"></a>
The main findings of the code can be found at the post available [here](https://sawy89.medium.com/do-promotional-offers-can-buy-you-a-coffee-49398f6079fe).

## Acknowledgements<a name="final"></a>

Must give credit to Starbucks and Udacity for the data, and the interesting subject




