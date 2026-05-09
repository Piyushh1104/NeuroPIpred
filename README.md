# NeuroPIpred: Prediction, Design and Scan of Insect Neuropeptides

## Overview

NeuroPIpred is a machine learning-based computational platform developed for predicting, designing, and scanning insect neuropeptides.

The platform uses experimentally validated natural and modified insect neuropeptides for building predictive models.

NeuroPIpred can:

- Predict insect neuropeptides
- Design mutant neuropeptide analogs
- Scan proteins for neuropeptide regions
- Perform similarity search using BLAST

---

## Research Paper

**Title:** NeuroPIpred: a tool to predict, design and scan insect neuropeptides

**Authors:**  
Piyush Agrawal, Sumit Kumar, Archana Singh, Gajendra P. S. Raghava, and Indrakant K. Singh

**Journal:** Scientific Reports (2019)

**DOI:** https://doi.org/10.1038/s41598-019-41538-x
https://doi.org/10.5281/zenodo.20092837
---

## Background

Insect neuropeptides are signaling molecules that regulate:

- Mating
- Migration
- Oviposition
- Metabolism
- Growth and development
- Homeostasis

These peptides are promising targets for insect pest control and insecticide development.

---

## Dataset Information

Two datasets were developed:

### NeuroPIpred_DS1

- 875 unique natural insect neuropeptides
- Random SwissProt peptides as negative dataset

### NeuroPIpred_DS2

- 2024 modified neuropeptides with C-terminal amidation
- Modified peptides from SATPDB as negative dataset

---

## Machine Learning Algorithms

The following techniques were used:

- Support Vector Machine (SVM)
- Random Forest
- SMO
- J48 Decision Tree
- Naive Bayes

---

## Input Features

### Amino Acid Composition

Residue frequency-based features.

### Dipeptide Composition

Captures residue composition and local residue order.

### Binary Profiles

Encodes residue order and positional information.

### Split Composition

Uses N-terminal and C-terminal residues separately.

---

## Best Performing Models

### NeuroPIpred_DS1

Dipeptide composition based SVM model:

- Validation Accuracy: 83.71%
- MCC: 0.67

### NeuroPIpred_DS2

Dipeptide composition based SVM model:

- Validation Accuracy: 97.93%
- MCC: 0.96

---

## Important Residues

### Natural Neuropeptides

Residues enriched:

- C
- D
- F
- G
- N
- S
- Y

### Modified Neuropeptides

Residues enriched:

- D
- E
- F
- G
- M
- N
- P
- R
- S
- Y

---

## Motif Analysis

Important motifs identified:

### Natural Neuropeptides

- ECC
- QCK
- FDEI
- EIDR

### Modified Neuropeptides

- GPR
- SFGL
- WFGP
- YSF

---

## Web Server Modules

### Predict

Predicts neuropeptides from peptide sequences.

### Design

Generates mutant analogs for activity optimization.

### Protein Scan

Identifies possible neuropeptide regions in proteins.

### BLAST

Finds similar experimentally validated neuropeptides.

### Download

Allows downloading benchmark datasets.

---

## Technologies Used

- SVM_light
- WEKA
- Random Forest
- MERCI
- PSI-BLAST

---

## Applications

NeuroPIpred can be used for:

- Insect neuropeptide discovery
- Pest control research
- Peptide engineering
- Bioactive peptide design
- Insecticide development

---

## Performance Comparison

| Method | Accuracy | MCC |
|--------|----------|------|
| NeuroPID | 52.57% | 0.16 |
| NeuroPIpred | 83.71% | 0.67 |

---

## Availability

Web Server:

https://webs.iiitd.edu.in/raghava/neuropipred/

Docker Image:

raghavagps/gpsrdocker

---

## Contact

### Prof. Gajendra P. S. Raghava

Department of Computational Biology  
Indraprastha Institute of Information Technology Delhi  
New Delhi, India

Email: raghava@iiitd.ac.in

---

## License

Creative Commons Attribution License

---

Generated from the uploaded NeuroPIpred research paper.
