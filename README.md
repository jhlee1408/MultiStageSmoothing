# MultiStageSmoothing
This repository contains the code for simulations and data examples in our paper on multi-stage smoothing methods for dynamic network estimation.

Nonparametric estimation of time-varying network connections by multi-stage smoothing, by Jeonghwan Lee, Tianxi Li, and Adam J. Rothman.

Abstract: We consider the problem of estimating the underlying edge probabilities of a time-varying network observed at multiple time points. The probability structure is represented by a time-varying graphon that satisfies temporal Hölder smoothness and piecewise Lipschitz conditions in the latent variables. We propose a multi-stage smoothing estimator that first applies temporal local smoothing to each edge and then performs node-domain smoothing using a data-driven neighborhood construction. An additional temporal smoothing step is introduced as an optional refinement when uniform accuracy over the entire time domain is required. Simulation studies demonstrate the benefits of combining temporal and node-domain smoothing under different generative models. We also apply the method to a real time-varying network dataset and show that it captures both smooth temporal evolution and structural patterns in the connectivity. 


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

