# RVFL

This repository contains code for enhancing the **Random Vector Functional Link (RVFL)** model using **small-world connectivity**, **Bayesian pruning**, and **robust initialization strategies**.

## Directory Structure
RVFL/
├── CorrRVFL/ 
│ └── P1.ipynb 
| └── P2.ipynb 
│
├── Vanilla_RVFL_and_variants/ 
│ ├── dynamic_masking.ipynb
│ └── autoencoder_init.ipynb
│
└── README.md 

### `P1`: CorrRVFL Exploration

* Explores the custom **CorrRVFL** model on regression datasets.
* Tests different optimization methods such as **Nesterov Gradient Descent (NAG)** and **Adam**.
* Performs grid search over key hyperparameters.
* Compares CorrRVFL performance against **Vanilla RVFL**.

### `P2`: Dynamic Masking & Sparse Autoencoder

* Adds **dynamic masking** to both **SW-SP-RVFL** and **SW-SP-RVFL (Hidden + Direct)** variants.
* Incorporates a **sparse autoencoder** for informed RVFL weight initialization by reconstructing input features.
* Aims to move from random to more meaningful weight initialization.

### `RVFL`: Baseline Model and Variant Prototyping

* Provides an exploratory baseline for **Vanilla RVFL**.
* Evaluates RVFL on basic datasets.
* Introduces **sparse** and **small-world** structures into the model (SW-SP-RVFL variants).
* Includes a limited grid search due to computational constraints, with fixed masking parameters.

### `Small_world_RVFL_variants`: Full Evaluation of SW-SP-RVFL Variants

* Contains the final pipeline for evaluating **SW-SP-RVFL** and its variants.
* Performs **exhaustive grid search** over model parameters, mask settings, and pruning mechanisms.
* Focuses solely on **sparse** and **small-world** connectivity enhancements to RVFL.
