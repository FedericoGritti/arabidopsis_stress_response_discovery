# Arabidopsis Stress-Response Discovery: Notebook Section Titles

## 1. Phase 1: Bulk RNA-seq & Differential Expression (The "What")

### 1.1 Data Retrieval via GEOquery
### 1.2 Filtering Lowly Expressed Genes (CPM > 0.5)
### 1.3 Normalization for Composition Bias (TMM)
### 1.4 Exploratory Data Analysis (MDS Plots & Heatmaps)
### 1.5 Generalized Linear Model (GLM) & Likelihood Ratio Test (LRT)

## 2. Phase 2: Single-Cell RNA-seq Integration (The "Where")

### 2.1 Quality Control (mtRNA < 5% & nFeature Filter)
### 2.2 Log-Normalization & Variance Stabilization
### 2.3 Principal Component Analysis (PCA)
### 2.4 UMAP Visualization & SNN Clustering
### 2.5 Cluster Identification (Marker Genes)

## 3. Phase 3: Network Medicine & Propagation (The "How")

### 3.1 Mapping Genes to the Interactome (STRING/AraPPINet)
### 3.2 Identifying the Largest Connected Component (LCC)
### 3.3 Calculating Average Shortest Path Length
### 3.4 Random Walker Propagation

## 4. Phase 4: Functional Validation

### 4.1 Gene Ontology (GO) & Pathway Enrichment (KEGG)
