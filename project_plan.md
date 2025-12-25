

# Project Checklist: Arabidopsis Salinity-Stress Systems Biology

## Phase 1: Bulk RNA-seq & Differential Expression (The "What")

*Goal: Identify the transcriptome-wide signature of Arabidopsis root response to Salt.*

* [x] **Data Retrieval (GSE158525 via GEOquery)**
* **Why:** To study *Arabidopsis thaliana* roots treated with 150mM NaCl, providing a high-quality baseline for salinity response.


* [ ] **Filtering Lowly Expressed Genes (CPM > 0.5)**
* **Why:** To remove transcriptional noise; genes not expressed in roots shouldn't interfere with the statistical model.


* [ ] **TMM Normalization for Plant Composition Bias**
* **Why:** Salt stress significantly alters plant cell metabolism; TMM ensures that a few highly upregulated stress genes don't mask the rest of the transcriptome.


* [ ] **Exploratory Data Analysis (MDS Plots)**
* **Why:** To confirm that the "Salt" samples group together and are biologically distinct from "Control" roots.


* [ ] **Likelihood Ratio Test (LRT) for Salt-Responsive DEGs**
* **Why:** To identify the set of genes significantly induced or repressed by NaCl using a Negative Binomial model.



## Phase 2: Single-Cell RNA-seq Integration (The "Where")

*Goal: Map the salt response to specific Arabidopsis root cell types (e.g., Epidermis vs. Stele).*

* [ ] **Quality Control (Plant-specific mtRNA & Chloroplast Filters)**
* **Why:** To remove damaged protoplasts; in roots, we monitor mitochondrial percentages to ensure cell viability.


* [ ] **Normalization & Variance Stabilization**
* **Why:** To compare gene expression across rare cell types (like the Quiescent Center) and abundant ones (like Cortex).


* [ ] **UMAP Visualization of Root Cell Atlas**
* **Why:** To visualize the spatial organization of the root in 2D space based on gene expression.


* [ ] **Cluster Identification via Marker Genes**
* **Why:** To identify which specific tissues (Xylem, Phloem, Endodermis) are most sensitive to salinity.



## Phase 3: Network Medicine & Propagation (The "How")

*Goal: Use the Arabidopsis Interactome to find hidden stress-response regulators.*

* [ ] **Mapping DEGs to the AraPPINet / STRING Interactome**
* **Why:** To transition from a list of "Salt genes" to a physical map of protein interactions in the plant cell.


* [ ] **Identifying the Salt-Stress Module (LCC)**
* **Why:** To test if salt-responsive proteins physically interact more than expected, forming a coherent biological machine.


* [ ] **Network Propagation (Python Random Walker)**
* **Why:** To identify "Hidden Players"—genes that don't change in expression but are critical "hubs" for salinity signaling.



## Phase 4: Functional Validation & Plant Physiology

* [ ] **GO Enrichment (Biological Process: Response to Salt Stress)**
* **Why:** To statistically prove our results are linked to known salinity pathways like Abscisic Acid (ABA) signaling.



