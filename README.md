# Using Data Science Techniques for SCIN Data Set

The SCIN (Skin Condition Image Network) open access dataset aims to supplement publicly available dermatology datasets from health system sources with representative images from internet users. To this end, the SCIN dataset was collected from Google Search users in the United States through a voluntary, consented image donation application. The SCIN dataset is intended for health education and research, and to increase the diversity of dermatology images available for public use.

The SCIN dataset contains 5,000+ volunteer contributions (10,000+ images) of common dermatology conditions. Contributions include Images, self-reported demographic, history, and symptom information, and self-reported Fitzpatrick skin type (sFST). In addition, dermatologist labels of the skin condition and estimated Fitzpatrick skin type (eFST) and layperson estimated Monk Skin tone (eMST) labels are provided for each contribution.

The data is stored in the [dx-scin-public-data bucket on Google Cloud Storage](https://console.cloud.google.com/storage/browser/dx-scin-public-data). Check out the [`load_SCIN.ipynb`](load_SCIN.ipynb) notebook for a quick review of how to access the dataset and the (Dataset Description) for an overview of its schema.

Please note: This dataset contains images of medical conditions, some of which may be sensitive and/or graphic in nature.

## Known issues:

* There are 15 images that are duplicates (and appear 42 times total) in the data. Because this data was used for the paper, it's been included in the release.
* There are 48 cases where the case is marked as gradable but no skin condition
  label is present. This happens for cases where they were marked as ungradable
  due to multiple conditions present.
* [Issue #1](https://github.com/google-research-datasets/scin/issues/1): 1 image file is missing


## Data Science Life Cycle:
*   Defining SCIN Data Set
* 	Defines Global Parameters for GCP
*   Dataset Schema
*   Intialize Google Cloud Storage client to Load CSV label files
*   Display the random images
*   Identify Invalid Images
*   Reverse Engineering
*   Drop One Hot Encoded Columns
*   Feature Engineering
*   Impute Missing Values & Fix Unbalanced Data
*   Dropping Unneeded Columns
*   Feature Engineering Part 2
*   Rename the Columns and its Values
*   Build Neural Network Model
*   Data Visualization\

---


## To access the Documentation that contains a step by step guide click [HERE](https://github.com/sahermuhamed1/Predictive-Modeling-for-Skin-Condition-Image-Network-SCIN-/blob/main/Data%20Preprocessing%20Documentation.docx)

## To access the Data Before Preprocessing click [HERE](https://github.com/sahermuhamed1/Predictive-Modeling-for-Skin-Condition-Image-Network-SCIN-/blob/main/Original_dataset.csv)

## To access the Data After Preprocessing click [HERE](https://github.com/sahermuhamed1/Predictive-Modeling-for-Skin-Condition-Image-Network-SCIN-/blob/main/Preproccessed_dataset.csv)

## To access the 15 Valid Records click [HERE](https://github.com/sahermuhamed1/Predictive-Modeling-for-Skin-Condition-Image-Network-SCIN-/blob/main/Val_Samples.csv)

## There is Two Notebooks I Used:

*  First Notebook is for data preproccessing and handeling the *Structured Data*, to acces it click [HERE](https://github.com/sahermuhamed1/Predictive-Modeling-for-Skin-Condition-Image-Network-SCIN-/blob/main/scin_notebook.ipynb)
*  Second Notebook is for image preprocessing and validate records, to access it click [HERE](https://github.com/sahermuhamed1/Predictive-Modeling-for-Skin-Condition-Image-Network-SCIN-/blob/main/preprocessing.ipynb)



