# CHE 4230 Tennessee Eastman Project

This project follows the CHE 4230 brief and uses the Tennessee Eastman data as a process-automation proxy for acetic acid production via oxidation of acetaldehyde.

TEP00 is treated as normal. TEP01–TEP15 are treated as faulty.

All files were harmonized to the common-sensor subset of 50 sensors because TEP11 had fewer columns and TEP14 included a text header row.

For computational stability inside this environment, the manifold-style unsupervised visualizations and clustering comparisons are run on a balanced stratified subset (up to 30 samples per fault class). EDA and supervised models use the full harmonized dataset.

Requested methods that were not directly available as native packages are delivered as clearly labeled fallback embeddings:
- UMAP-style fallback: SpectralEmbedding
- PaCMAP-style fallback: Isomap
- TriMAP-style fallback: MDS
