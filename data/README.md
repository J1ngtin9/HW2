## SustainBench – Poverty Change (LSMS) — Sample (≈120 words)
This folder contains a small sample (≤200 rows) extracted from the SustainBench
**poverty_change** task based on the World Bank LSMS panel surveys. LSMS provides
nationally representative household data; SustainBench aggregates to the cluster
(enumeration area) level and builds PCA-based measures of asset change over time.
For this assignment we include **sample.csv** only to verify environment setup,
file I/O and quick plots. The full dataset (including paired Landsat bands and a
nightlights band per image, plus standardized splits) is large and should not be
committed here. Please follow the official SustainBench instructions to obtain
complete data and read the license/terms before running full experiments.

**Official source:** SustainBench – poverty_change (LSMS-based)  
**License/Terms:** See SustainBench/LSMS documentation; cite appropriately.

### Data Dictionary (sample.csv)
| variable_name   | type        | description                                      |
|-----------------|-------------|--------------------------------------------------|
| country         | string      | Country of the cluster                           |
| cluster_id      | string/int  | Cluster (enumeration area) identifier            |
| year.x          | int         | Earlier survey year for the pair                 |
| year.y          | int         | Later survey year for the pair                   |
| lat / lon       | float       | Cluster centroid (approx.)                       |
| lsms_id.x       | string/int  | Household ID at the earlier year (if present)    |
| lsms_id.y       | string/int  | Household ID at the later year (if present)      |
| diff_of_index   | float       | Δ(asset index) across years (diffOfIndex)        |
| index_of_diff   | float       | PCA of asset-differences (indexOfDiff)           |
| asset_index.x   | float       | Asset index at earlier year                      |
| asset_index.y   | float       | Asset index at later year                        |
| n               | int         | # of surveyed households in the cluster          |

