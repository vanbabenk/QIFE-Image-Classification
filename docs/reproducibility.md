# Reproducibility Notes

This document summarizes the reproducibility protocol for the QIFE image classification repository.

## Current notebook coverage

The current notebooks included in this repository reproduce the MNIST experiments:

- `notebooks/01_QIFE_MNIST.ipynb`
- `notebooks/02_QFE_Baseline_MNIST.ipynb`
- `notebooks/03_CNN_Baseline_MNIST.ipynb`

If the manuscript reports Fashion-MNIST experiments, add corresponding notebooks or convert the current notebooks into dataset-configurable versions.

## Experimental protocol

- Dataset: MNIST
- Number of classes: 10
- Balanced training subset: 1,200 images per class, 12,000 images in total
- Balanced testing subset: 200 images per class, 2,000 images in total
- Image size: 22 × 22
- Patch size: 3 × 3
- Patch stride: 2
- Number of patches per image: 100
- Number of patch values: 9
- Optimizer: Adam
- Learning rate: 0.0005
- Batch size: 64

## Execution environment

The notebooks are intended to be executed in Google Colab.

Recommended validation procedure:

1. Open the notebook from GitHub using the Colab badge.
2. Select `Runtime → Disconnect and delete runtime`.
3. Reconnect to a fresh runtime.
4. Select `Runtime → Run all`.
5. Confirm that no Google Drive file or private path is required.
6. Confirm that metrics and confusion matrix are generated.

## Quantum simulation note

The QIFE and QFE notebooks use PennyLane with a simulator backend. The results should not be interpreted as direct execution on a real quantum processing unit.

## Publication checklist

Before citing this repository in the manuscript:

- Verify that the QIFE, QFE, and CNN notebooks use exactly the same experimental settings.
- Verify whether `max_iterations` matches the manuscript protocol in every notebook.
- Confirm that all notebooks run on a clean Colab runtime.
- Upload raw and summary metric CSV files into `results/`.
- Create a GitHub release, e.g. `v1.0.0`.
- Archive the release on Zenodo if a DOI is required.
