# BPQ_RNA

A Hybrid quantum-classical pipeline for predicting RNA secondary structures, including post-transcriptional modifications, using a native base-pair-level Quadratic Unconstrained Binary Optimization (QUBO) formulation.

The contents of this repository are part of the work titled:
## A Thermodynamically Informed Base-pair QUBO for RNA Secondary Structure Prediction including Post-transcriptional Modifications

**Authors:** Nivedita Dutta, Quentin Vicens, and Liwen Shih

BPQ_RNA is a hybrid quantum-classical framework for predicting RNA secondary structures using a natively base-pair-level Quadratic Unconstrained Binary Optimization (QUBO) formulation. By mapping experimental Nearest Neighbor Database (NNDB) free energies directly onto the Hamiltonian, we bypass coarse-grained pre-assembly. This code executes exact classical baselines, quantum optimization via QAOA (tracking algorithmic tunneling convergence), and a classical maturation post-processing layer to resolve the energetic consequences of loops and dangling ends.

## Google Colab Notebook

The BPQ_RNA Colab notebook can be accessed here: [BPQ_RNA](https://colab.research.google.com/drive/1Cq4usbkZ2FW9y0_sZ1hvk12XFBa-vkpW?authuser=1#scrollTo=QyusiFCFcslu)

**Citation:** Dutta, N., Vicens, Q., and Shih, L. A Thermodynamically Informed Base-pair QUBO for RNA Secondary Structure Prediction including Post-transcriptional Modifications.

## Free Energy Parameters

The experimentally derived Free energy parameters in efficiently utilizable formats are provided here: [Free Energy Parameters Gist](https://gist.github.com/duttan710/1429a1150dcd7d75fb5ca0cf29b92963/)

When you use BPQ_RNA, please also cite:

1. Turner, D. H. & Mathews, D. H. (2009). NNDB: The nearest neighbor parameter database for predicting stability of nucleic acid secondary structure. *Nucleic Acids Research*, 38, D280-D282.
2. Mittal, A., Turner, D. H., & Mathews, D. H. (2024). NNDB: An Expanded Database of Nearest Neighbor Parameters for Predicting Stability of Nucleic Acid Secondary Structures. *Journal of Molecular Biology*, 168549.
3. Kierzek, E., Zhang, X., Watson, R.M. et al. (2022). Secondary structure prediction for RNA sequences including N6-methyladenosine. *Nat Commun*, 13, 1271.
