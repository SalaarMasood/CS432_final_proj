
# EDA Observations — GAD-NR Datasets

## inj_cora
- Anomaly type: INJECTED (synthetic, both structural + contextual).
- <fill in> anomaly ratio computed from data: X.X% (compare to paper's ~11%).
- 1433 features: PCA explained variance is low (~X%), indicating high dimensionality.
- Degree distribution: anomalous nodes show [higher/lower/similar] degree vs normal.
- PCA: [visible/no visible] separation of anomalous nodes — consistent with contextual injection.

## Weibo
- Anomaly type: ORGANIC contextual (social network spambots).
- Highest anomaly ratio among all 6 datasets: 10.3%. Easiest to visualize.
- 407,918 edges makes this the densest graph — avg degree = ~97.
- PCA: [expect visible separation — contextual anomalies differ in feature space].
- Degree distributions of normal vs anomalous nodes [overlap / are distinct].

## Reddit
- Anomaly type: STRUCTURAL (anomalous posting/commenting patterns).
- 64 features; correlation heatmap shows [describe pattern] for normal vs anomalous.
- PCA: [expect NO separation — structural anomalies are not detectable by features alone].
- Degree distribution: anomalous nodes show [describe observation].
- This dataset motivates neighborhood-based detection (GAD-NR's approach).

## Enron
- Anomaly type: STRUCTURAL (known fraudsters in the Enron email network).
- EXTREME class imbalance: only 5 anomalies in 13,533 nodes (0.04%).
- Standard accuracy metric would score 99.96% by predicting all-normal — illustrates why AUC is used.
- The 5 anomalous nodes have degrees: [list actual values from degree plot].
- Feature correlation heatmaps: [describe if anomalous correlation pattern differs].
