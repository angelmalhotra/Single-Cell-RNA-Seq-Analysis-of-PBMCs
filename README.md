# Single-Cell-RNA-Seq-Analysis-of-PBMCs

My Single-Cell Analysis Project: PBMCs

My full bioinformatics project where I analyzed a single-cell RNA-seq dataset from start to finish. I was really excited to see if I could take a public dataset of human immune cells and figure out what different cell types were in the sample using Python.

The Data
I used a popular public dataset from 10x Genomics of 3,000 Peripheral Blood Mononuclear Cells (PBMCs) from a healthy donor.

Analysis Workflow
The analysis pipeline consisted of the following key steps:
- **Quality Control (QC):** Filtering out low-quality cells based on metrics like gene count and mitochondrial DNA percentage.
- **Data Normalization and Transformation:** Correcting for cell library size and applying a log transformation to stabilize variance.
- **Feature Selection:** Identifying the top ~2,000 highly variable genes (HVGs) to focus the analysis on biologically informative signals.
- **Dimensionality Reduction:** Using Principal Component Analysis (PCA) and Uniform Manifold Approximation and Projection (UMAP) to visualize the data in 2D.
- **Clustering:** Applying the Leiden community detection algorithm to group similar cells together.
- **Cell Type Annotation:** Identifying the biological identity of each cluster by finding and visualizing canonical marker genes.

What I Learned//Key Skills
- **Programming:** Python, Scanpy, Pandas, Matplotlib
- **Bioinformatics:** Single-Cell RNA-Seq (scRNA-seq) Analysis, Quality Control, Normalization, Feature Selection, Dimensionality Reduction, Clustering.
- **Biology:** Identification of immune cell types (T-cells, B-cells, Monocytes, NK cells) using marker genes.=

Final Result
The final annotated UMAP shows the successful identification of all major expected cell populations:

![Final Annotated UMAP Plot](final_umap_plot)
