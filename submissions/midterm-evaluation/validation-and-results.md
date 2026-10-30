# Validation and Results

The approved binary model metadata records a held-out PortScan test split. Integration smoke tests demonstrated:

- 100 benign rows returned 100 `BENIGN` predictions.
- 100 labelled PortScan rows returned 99 `PortScan` and 1 `BENIGN` prediction.

These smoke tests validate the application path. They are not independent production performance evidence because the data comes from the same source dataset family.