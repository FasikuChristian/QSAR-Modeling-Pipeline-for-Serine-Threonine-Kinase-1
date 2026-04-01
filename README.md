# QSAR Modeling Pipeline for AKT Inhibitors

## Introduction

This repository presents a reproducible QSAR modeling workflow to predict AKT inhibitory activity using molecular descriptors and fingerprints. The pipeline integrates feature engineering, machine learning, and validation to build predictive models for drug discovery and computational chemistry research.

The workflow is adapted from publicly available tutorial materials and substantially extended with new datasets, preprocessing steps, multiple machine learning algorithms, and rigorous validation.

## Project Objectives

* Develop predictive QSAR models for AKT inhibitors
* Generate molecular descriptors and fingerprints
* Train and compare multiple machine learning models
* Validate models using cross-validation
* Provide a reproducible and transparent workflow

## Workflow Overview

Data Collection → Descriptor & Fingerprint Generation → Preprocessing → Feature Selection → Model Training → Cross-Validation → Model Evaluation → Prediction

## Dataset

* Target: AKT (Protein Kinase B)
* Endpoint: Biological activity (IC50/pIC50)
* Format: CSV with SMILES and activity
* Source: ***ChEMBL database  ******[https://www.ebi.ac.uk/chembl/](https://www.ebi.ac.uk/chembl/)***

## Feature Generation

* **Descriptors:** PaDEL and RDKit for physicochemical and structural properties (MW, LogP, H-bond donors/acceptors, TPSA, rotatable bonds)
* **Fingerprints:**  structural fingerprints encoding molecular substructures

## Preprocessing & Feature Selection

* Handle missing values
* Remove low-variance and highly correlated features
* Standardize features for algorithm performance

## Machine Learning Models

* Random Forest
* XGBoost
* CatBoost
* K-Nearest Neighbors (KNN)

## Validation

* Cross-validation for model stability
* Train/test split for generalization
* Metrics: R², RMSE, MAE, Q²

## Repository Structure

```
akt-qsar-model/
├── data/
├── descriptors/
├── scripts/  
├── models/
├── results/
├── requirements.txt
├── README.md
└── LICENSE
```

## Running the Pipeline


## Key Contributions

* New AKT dataset
* Molecular descriptors and fingerprints
* Removal of highly correlated features
* Training multiple ML models (Random Forest, XGBoost, CatBoost, KNN)
* Cross-validation and performance evaluation

## Reproducibility

* Fixed random seed
* Documented preprocessing steps
* Saved model parameters
* Dependencies listed in requirements.txt

## Acknowledgment

Adapted from tutorial and github page developed by the Data Professor: [https://github.com/dataprofessor/code](https://github.com/dataprofessor/code)

## Author

Fasiku Christiian Ayobami — Computational Chemistry / QSAR Modeling

## License

Licensed under Apache License 2.0
