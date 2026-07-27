# Results

This folder is prepared for reproducibility outputs.

Recommended files:

- `raw_metrics.csv`: per-method, per-dataset, per-seed results.
- `summary_metrics.csv`: mean and standard deviation for each metric.
- `runtime_summary.csv`: runtime information, if reported in the manuscript.

Suggested columns for `raw_metrics.csv`:

```text
method,dataset,seed,test_loss,accuracy,precision,recall,f1,auc,runtime_seconds
```

Do not upload large datasets or model checkpoints to this folder.
