# Phase III — Implementation

## Components

| Component | Purpose |
| --- | --- |
| Dashboard | analysis, alerts, model, and report views |
| FastAPI service | local CSV inference endpoints |
| Rule and ML script | offline hybrid CSV workflow |
| Live capture | bounded TCP/UDP connection metadata |
| Submission documents | reproducible academic evidence |

The live-capture component intentionally marks rows **Not evaluated** rather than attaching unvalidated model verdicts.