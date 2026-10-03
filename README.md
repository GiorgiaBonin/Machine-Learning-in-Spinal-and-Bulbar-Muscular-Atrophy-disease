# Machine Learning for Brain MRI Analysis in Spinal and Bulbar Muscular Atrophy

This repository accompanies Giorgia Bonin's Master's thesis in Data Science at the University of Padua (academic year 2026–2026). It contains the thesis report and the presentation prepared for the thesis defense.

## Overview

The thesis investigates whether SBMA affects structural cortical gray-matter in impaired individuals. Specifically it tests (1) whether it's possible to distinguish different cortical regions organization between spinal and bulbar mascular athrophy (SBMA) and healthy individuals and (2) whether it's possible to correctly classify individuals in the 2 cohorts by looking at T2-weighted brain MRI. To answer the questions the thesis combines unsupervised community-detection analysis and supervised classification with explainable AI methods.
The study analyzed 38 scans: 20 from participants with SBMA and 17 from healthy controls. Cortical gray matter was summarized across 1,000 Schaefer parcels. 
A graph-based pipeline compared cohort-level parcel communities using Leiden clustering and consensus clustering to answer question (1).
A supervised pipeline compared raw and total-gray-matter-normalized regional measures, selected features within leave-one-out cross-validation, evaluated several classifiers, and used SHAP to examine regional contributions to answer question(2).

In the reported experiments:
- (1) there is a broad agreement in cortical gray matter organization between the cohors with small differences localized in the lefty somatomotor cortex.
- (2) It's possible to distinguish SBMA from healthy individuals when looking at normalized regional gray-matter. L2-regularized logistic regression had the strongest overall balance, with accuracy and F1-score of 0.84.

## Documents

- `Bonin_Giorgia_Master_Thesis.pdf` — complete thesis report.
- `SBMA_Thesis_Presentation.pdf` — thesis defense presentation.

## Code and data

The analysis code is available upon request. Individual-level MRI data are not included in this repository.

## Author and acknowledgments

**Author:** Giorgia Bonin, Master's degree in Data Science, University of Padua.

The thesis was supervised by Professor Francesco Rinaldi. 

