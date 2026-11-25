# Philippine Province-Level Typhoon Impact-Risk Classification
## End-to-end research notebook | XGBoost · GRU · ResNet-18 · Multimodal Fusion

**Research question:** Can historical typhoon track, exposure, and vulnerability information classify the severity of observed impacts at the Philippine province and storm level?

**Read first:** This notebook records a retrospective research experiment, not an operational forecasting system. The saved outputs predate the expanded weather, terrain, poverty and housing features; rerun the notebook before interpreting them as expanded-model results. The saved run uses  Digital Typhoon matches, UTC image timestamps and interpolated first-landfall anchors; The test split has previously been inspected, so its comparisons are exploratory. Historical best-track records do not establish real-time data availability.

**Workflow:** 0 configuration → 1 source audits & EDA → 2 matching and cutoff → 3 storm-group splits and outcome labels → 4 features → 5 XGBoost → 6 GRU → 7 ResNet-18 → 8 fusion and tuning → 9 evaluation → 10 export.
