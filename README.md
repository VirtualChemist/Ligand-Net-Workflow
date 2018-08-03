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
* sklearn
* mayachemtools
* A folder looking like this:

<img src="https://github.com/dcastaneda5/Ligand-Net-Workflow/blob/master/folder.png" height="240">

The actives folder should contain at least one `.txt` or `.sdf` file. The decoys folder should contain at least one `.txt` or `.sdf` file as well. Each protein **MUST** have a decoys and an actives file **WITH THE _SAME_ NAME** but found in different folders, for example: /Users/Daniel/Desktop/ligand_net/actives/thromboxane_a2_receptor.txt **AND** /Users/Daniel/Desktop/ligand_net/decoys/thromboxane_a2_receptor.txt
If the files for the decoys and actives do not have the same name, the program will not be able to generate a machine learning model.

In case you don't have a file for the active ligands, we recommend you running the `looking_actives.py` code found in this repository. Said code needs an accession number (which you can find in the [Pharos website](https://pharos.nih.gov/idg/targets)) of the desired protein. To see how to run this code, please refer to our **Fetching Ligands and Decoys** section.

In case you don't have a file for decoys (either in `.txt` or `.sdf`), you may download them through the [DUD-E website decoy generator](http://dude.docking.org/generate) or by using the [DecoyFinder software](http://urvnutrigenomica-ctns.github.io/DecoyFinder/#Downloads_). The latter uses the ZINC database to find a specific number of decoys set by the user; to see how to use it, please refer to our **Fetching Ligands and Decoys** section.

If you don't know how to install any of these packages/modules, please refer to the **Installation** section (below).
## Installation
First, we need to create a Conda python environment. For this, follow the next steps:
1. Install Anaconda 3 from [here](https://www.anaconda.com/download/#linux)
2. Create a new python environment in your terminal:
`conda create -n <env_name> python=3.5 anaconda
source activate <env_name>`
(where <env_name> is whatever name you want to give your environment).

For the installation of the remaining packages/modules, keep working in your terminal with the activated environment. Then do:
3. `conda install -c rdkit rdkit`
4. `conda install -c conda-forge tqdm`
5. `conda install -c anaconda scikit-learn`
6. Install [mayachemtools](http://www.mayachemtools.org/Download.html) and copy the directory in the folder you created with the other directories shown on the previous image. Once untared and unzipped, you should be able to move to that directory (i.e. cd /Users/Daniel/Desktop/ligandnet/mayachemtools/). Inside said folder you should have something like this:



## Fetching Ligands and Decoys

## Running the tests

## Authors

## Contributions

## Acknowledgments





