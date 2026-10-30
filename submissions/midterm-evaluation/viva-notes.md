# Mid-Term Viva Notes

**Why hybrid?** Rules provide explainable evidence; the classifier identifies patterns in the approved feature space.

**Does it detect every attack?** No. The connected model is limited to the approved `BENIGN` versus `PortScan` CSV scope.

**Why not classify live traffic?** Raw packets must first become validated flow features matching the trained model. Guessing those features would create misleading alerts.