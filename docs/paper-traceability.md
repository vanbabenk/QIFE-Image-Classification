# Paper Traceability

This document maps manuscript components to repository files.

| Manuscript component | Repository file | Notes |
|---|---|---|
| Proposed QIFE method | `notebooks/01_QIFE_MNIST.ipynb` | Implements the QIFE pipeline with patch-level quantum feature extraction. |
| QFE baseline | `notebooks/02_QFE_Baseline_MNIST.ipynb` | Implements the QFE baseline comparison. |
| Classical CNN baseline | `notebooks/03_CNN_Baseline_MNIST.ipynb` | Implements the classical CNN baseline. |
| Method flowchart | `docs/figures/qife_flowchart.png` | Visual description of the QIFE workflow. |
| Experimental protocol | `docs/reproducibility.md` | Documents dataset, preprocessing, and execution environment. |
| Reported results | `results/` | Store raw per-run metrics and summary statistics here. |

## Items to verify before final release

- The manuscript mentions MNIST and Fashion-MNIST, while the uploaded notebooks currently target MNIST.
- QFE and CNN notebooks use `max_iterations=1000`; the uploaded QIFE notebook should be checked because its current call uses `max_iterations=100`.
- If the final manuscript reports five independent runs, add the seed loop or provide the raw per-seed result files.
