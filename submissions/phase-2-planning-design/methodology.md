# Methodology

1. Audit CICIDS labels and select the approved `BENIGN` and `PortScan` scope.
2. Convert values to numeric form; handle missing and infinite values.
3. Persist the model, scaler, feature list, label encoder, and metadata as one versioned bundle.
4. Evaluate accuracy, precision, recall, F1, false-positive rate, and false-negative rate on a held-out split.
5. Keep rule triggers and ML predictions visible as separate provenance.

Any within-dataset result is reported as a validation measurement, not production detection accuracy.