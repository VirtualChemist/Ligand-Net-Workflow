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
<img src="https://github.com/favicon.ico" height="20">

Besides that, it is important that you have a file in .txt or .sdf format containing a set of known actives that bind to a specific protein, and a set of decoys. If you don't have a file for the actives, and you wish to get one in a `.sdf` format, we recommend you using the code `looking_actives_sdf.py` found in this repository. Said file needs an accession number (which you can find in the [Pharos website](https://pharos.nih.gov/idg/targets))after you type the name of the protein. If you wish to get a file with the ligands in SMILES and in `.txt` format, we suggest you to use the code `looking_actives_txt.py` instead. To see how to run these files, please refer to our **Fetching Ligands and decoys** section.

If you don't know how to install any of these packages/modules, please refer to the **Installation** section (below).
## Installation



