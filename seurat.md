---
layout: software_layout
title: Seurat
permalink: /seurat/
---

# About Seurat

Seurat is an R package designed for QC, analysis, and exploration of single cell RNA-seq data. It easily enables widely-used analytical techniques, including the identification of highly variable genes, dimensionality reduction (PCA, ICA, t-SNE), standard unsupervised clustering algorithms (density clustering, hierarchical clustering, k-means), and the discovery of differentially expressed genes and markers.

Seurat also features two recently developed computational methods for single cell analysis:

1. Unsupervised clustering and discovery of cell types and states [(Macosko, Basu, Satija et al., Cell, 2015)](http://www.cell.com/cell/abstract/S0092-8674(15)00549-8)
	* Updated approach: Combining dimensional reduction with graph-based clustering
	* [Tutorial: Unsupervised identification of immune cell types and biomarkers from 2,700 PMBCs (10X Chromium)]({{"get_started.html" | prepend: site.seurat_nav}})
	* [Command List](https://www.dropbox.com/s/y6kwho066vugjrg/pbmc33k.R?dl=1): Unsupervised identification of immune cell types from [33,000 PBMCs (10X Chromium)
		* [Download precomputed object](https://www.dropbox.com/s/4cams873t2azmpf/pbmc33k.Rda?dl=1)
	* [Command List](https://www.dropbox.com/s/n3t13kk4mmo1ggs/pancreas.R?dl=1): Unsupervised identification of pancreas cell types from 8,500 single cells (inDrop) [(Baron et. al., Cell Systems, 2016)](http://www.cell.com/cell-systems/abstract/S2405-4712(16)30266-6)
		* [Download precomputed object](https://www.dropbox.com/s/av5p7d3ro4m0fb5/pancreas.Rda?dl=1)
2. Spatial reconstruction of single cell data [(Satija\*, Farrell\* et al., Nature Biotechnology, 2015)](http://www.nature.com/nbt/journal/vaop/ncurrent/full/nbt.3192.html)
	* Infers the original location of a single cell based on its gene expression, and a spatial reference map
	* [Tutorial: Inferring spatial localization of single cells during Zebrafish embryogenesis]({{"old-get-started/" | prepend: site.seurat_nav}})

All methods emphasize clear, attractive, and interpretable visualizations, and were designed to be [easily used]({{"get_started.html" | prepend: site.seurat_nav}}) by both dry-lab and wet-lab researchers.

Seurat is developed and maintained by the Satija lab, in particular by [Andrew Butler](mailto:abutler@nygenome.org), [Christoph Hafemeister](mailto:chafemeister@nygenome.org), and [Shiwei Zheng](mailto:szheng@nygenome.org), and is released under the GNU Public License (GPL 3.0). We are also grateful for significant ideas and code from [Jeff Farrell](mailto:jfarrell@g.harvard.edu), [Karthik Shekhar](mailto:karthik@broadinstitute.org), and [other generous contributors]({{ "contact.html" | prepend: site.seurat_nav }}).


## News
**October 4, 2016:** Version 1.4 released

* Added methods for negative binomial regression and differential expression testing for UMI count data
* New ways to merge and downsample Seurat objects

**August 22, 2016:** Version 1.3 released

* Improved clustering approach - see FAQ for details
* All functions support sparse matrices
* Methods for removing unwanted sources of variation
* Consistent function names
* Updated visualizations

**May 21, 2015:**
[Drop-Seq manuscript](http://www.cell.com/cell/abstract/S0092-8674(15)00549-8) published. Version 1.2 released

* Added support for spectral t-SNE (non-linear dimensional reduction), and density clustering
* New visualizations - including pcHeatmap, dot.plot, and feature.plot
* Expanded package documentation, reduced import package burden
* Seurat code is now hosted on GitHub, enables easy install through devtools package
* Small bug fixes

**April 13, 2015:**
[Spatial mapping manuscript](http://www.nature.com/nbt/journal/vaop/ncurrent/full/nbt.3192.html) published. Version 1.1 released


