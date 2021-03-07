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
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

Not all users receive the same offer, and that is the challenge to solve with this data set.

The objective of the analysis is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

Every offer has a validity period before the offer expires. As an example, a BOGO offer might be valid for only 5 days. 

## File descriptions <a name="files"></a>

### Dataset
The dataset is in the made of three files, stored in the `/data` folder:
- `portfolio.json` - containing offer ids and meta data about each offer (duration, type, etc.)
- `profile.json` - demographic data for each customer
- `transcript.json` - records for transactions, offers received, offers viewed, and offers completed
Here is the schema and explanation of each variable in the files:

*portfolio.json*
id (string) - offer id
offer_type (string) - type of offer ie BOGO, discount, informational
difficulty (int) - minimum required spend to complete an offer
reward (int) - reward given for completing an offer
duration (int) - time for offer to be open, in days
channels (list of strings)

*profile.json*
age (int) - age of the customer
became_member_on (int) - date when customer created an app account
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
id (str) - customer id
income (float) - customer's income

*transcript.json*
event (str) - record description (ie transaction, offer received, offer viewed, etc.)
person (str) - customer id
time (int) - time in hours since start of test. The data begins at time t=0
value - (dict of strings) - either an offer id or transaction amount depending on the record

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




