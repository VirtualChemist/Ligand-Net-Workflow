# Ligand-Net-Workflow
This workflow helps the user to determine whether a set of ligands act as actives or decoys when it comes to bind to a specific protein.

## Getting Started
These set of instructions will help you understand and develop a Machine Learning (ML) model to predict ligands as actives or decoys. This workflow generates classification models based on different approach that the user may choose. Those include the following:

* Support Vector Machine (SVM)
* Random Forest (RF)
* Extra Tree Classifier (ETC)
* Neural Networks (NN)

You can either choose one approach to develop a classification model or you may choose all of them. Either way we will run different parameters to find the best model that fits your data; in other words, we will select the one that gives the highest Positive Predictive Value (PPV), sensitivity, and specificity.

## Prerequisites
We need you to have the following in your local computer:
* Anaconda
* Python 3.5 or above
* rdkit 
* tqdm
* numpy
* sklearn
* mayachemtools
* A folder looking like this:

<img src="https://github.com/dcastaneda5/Ligand-Net-Workflow/blob/master/folder.png" height="240">
The actives folder should contain at least one `.txt` or `.sdf` file. The decoys folder should contain at least one `.txt` or `.sdf` file as well. Each protein **must** have a decoys and an actives file **with the _same_ name** but found in different folders, for example: /Users/Daniel/Desktop/ligand_net/actives/thromboxane_a2_receptor.txt **and** /Users/Daniel/Desktop/ligand_net/decoys/thromboxane_a2_receptor.txt

In case you don't have a file for the active ligands, we recommend you running the `looking_actives.py` code found in this repository. Said code needs an accession number (which you can find in the [Pharos website](https://pharos.nih.gov/idg/targets)) of the desired protein. To see how to run this code, please refer to our **Fetching Ligands and decoys** section.

If you don't know how to install any of these packages/modules, please refer to the **Installation** section (below).
## Installation



