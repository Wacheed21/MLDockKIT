# MLDockKit
This is a simple platform for computing Lipinsky's Rule of five using the rdkit package, predicting pIC50 of canonical SMILES that are potential targets against Oestrogen receptor alpha protein as ant-prostate cancer agaents using a preformatted RandomForest model, and docking of the canonical SMILE with the Oestrogen receptor alpha protein using Audodock Vina package. 
### Purpose of the Package
The purpose of the package is to provide a unified platform for computing prostate cancer drug likeness indicess and performing docking on the same compounds. 
### Features
Important chemoinformatics features of Oestrogen receptor alpha antagonists such as:
    - Lipinsky descriptors
    - Prediction of pIC50
    - Docking and visiualization 
### Getting Started
The package is found on pypi hence can be installed with pip
#### Pre-requisites
Installation of Vina requires [boost](https://www.boost.org/doc/libs/1_83_0/tools/build/doc/html/index.html#bbv2.installation) and [swig](https://www.swig.org/)  
Importantly: Install pymol as the first package in the new environment, this is due to environmental package conflict.
#### Installation
It is important to ensure that all the required dependencies are installed in your working environment. It would be much easier if you create a conda environment before installation of packages. The following packages are required, **pymol**, **rdkit**, **pandas**, **gemmi**, **padelpy**, **joblib**,**openbabel**, **Autodock Vina**, **java**, **scipy**, **MDAnalysis** and **scikit-learn**.
```bash
conda create -n MLDockKit
conda activate MLDockKit
```

Then, install pymol before installing other packages:
```bash
conda install -c conda-forge pymol-open-source vina mdanalysis 

conda install -c cyclus java-jre

pip install MLDockKit
```
