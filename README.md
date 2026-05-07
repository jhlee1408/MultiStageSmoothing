# MultiStageSmoothing


# MultiStage Smoothing for Dynamic Network Estimation
This repository contains the code for simulations and data examples in our paper on multi-stage smoothing methods for dynamic network estimation.

The repository currently includes the following files:
- `MultiStage_main.R`  
  Main estimation and comparison methods, including the proposed multi-stage smoothing procedure, cross-validation routines, and benchmark methods.
- `MultiStage_helper.R`  
  Helper functions for simulations, error calculations, data generation, matrix norms, and auxiliary utilities used throughout the experiments.
- `MultiStage_simulation.R`  
  Parallel simulation script for reproducing the numerical experiments under multiple dynamic network models.
- `DataExamples_preprocessing.R`  
  Preprocessing pipeline for the real data examples analyzed in the paper.
- `DataExamples_analysis.R`  
  Main analysis script for reproducing the real data applications and figures.

## Data
Due to GitHub file size limits, the data files are hosted externally.
Data download link: [https://drive.google.com/drive/folders/1nA_NM5FmrM-yKd8eoylqY472G_Rl7zXm?usp=share_link]

## Notes
The simulation scripts are designed to reproduce the main numerical experiments in the paper, including:
- Dynamic stochastic block models (DSBM)
- Orthogonal DSBM settings
- Dynamic random dot product graph (RDPG) models
- Dynamic latent distance models

The benchmark methods implemented in the repository include:
- Proposed multi-stage smoothing method
- Reversed multi-stage smoothing
- FASE-based estimator
- Pensky-Zhang estimator
- Pooled smoothing estimator
- Independent neighborhood smoothing estimator

