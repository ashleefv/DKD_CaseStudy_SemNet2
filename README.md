# DKD_CaseStudy_SemNet2
Code for diabetic kidney disease (DKD) case study using SemNet 2.0.

[![DOI](https://zenodo.org/badge/740179121.svg)](https://zenodo.org/doi/10.5281/zenodo.10480080)

## Overview
This DKD case study was performed with SemNet 2.0 to identify pathophysiological processes associated with DKD through extensive biomedical text-mining. 

## Authors
Krutika Patidar<sup>a</sup>,  Jennifer H. Deng<sup>b</sup>, Cassie S. Mitchell<sup>b,c</sup>, Ashlee N. Ford Versypt<sup>a,d,e</sup> 

<sup>a</sup>Department of Chemical and Biological Engineering, University at Buffalo, The State University of New York, Buffalo, NY, USA<br/>
<sup>b</sup>Department of Biomedical Engineering, Georgia Institute of Technology and Emory University School of Medicine, Atlanta, GA, USA<br/>
<sup>c</sup>Center for Machine Learning at Georgia Tech, Georgia Institute of Technology, Atlanta, GA, USA<br/>
<sup>d</sup>Department of Biomedical Engineering, University at Buffalo, The State University of New York, Buffalo, NY, USA<br/>
<sup>e</sup>Institute for Artificial Intelligence and Data Science, University at Buffalo, The State University of New York, Buffalo, NY, USA<br/>


## Script

* DKD-SemNet-visualization.ipynb This is a Jupyter notebook (Python 3) used to visualize data provided in the following data files.

## Data files

* TOP10_combined_triple.csv This file contains the top 10% of source nodes associated with each pairwise domain (DKD, IR, GEC, KD, DB). Each source node has a name, semantic type (aapp or gngm), domain, mean HeteSim score, and count. 
* MGI_triple_aapp.csv This file contains mapped ontologies of the top 10% proteins (aapp) at the intersection of DKD, IR, and GEC domains.
* MGI_triple_gngm.csv This file contains mapped ontologies of the top 10% genes (gngm) at the intersection of DKD, IR, and GEC domains.

## Cytoscape session
* interaction-network-session.cys This saved Cytoscape session can be run using the Cytoscape (v3.10.0) software to generate the protein-protein (or protein-gene) interaction network. "PPI_network_paper" network in the session generates the PPI in the manuscript.
* interaction.sif This file contains interaction rules between proteins/genes.
* edge_rule.sif This file maps the positive (+1) or negative (-1) regulatory relation between interacting proteins as provided in interaction.sif. 

## Recommended Supplementary Packages
* [SemNet 2.0](https://github.com/pathology-dynamics/semnet-2) is a group of modules for working with semantic networks, specifically those built using the Semantic MEDLINE Database (SemMedDB) repository of semantic predications.
* [Cytoscape](https://cytoscape.org/) is an open-source software platform for visualizing complex networks and integrating these with any type of attribute data.
  
## Acknowledgements
This work was supported by National Institutes of Health grant R35GM133763 to A.N.F.V., National Science Foundation CAREER grant 2133411 to A.N.F.V., National Science Foundation CAREER grant 1944247 to C.M, National Institute of Health grant U19-AG056169 sub-award to C.M., and by the Chan Zuckerberg Initiative under grant 253558 to C.M. 
