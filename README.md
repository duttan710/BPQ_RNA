# BPQ_RNA

A Hybrid quantum-classical pipeline for predicting RNA secondary structures, including post-transcriptional modifications, using a native base-pair-level Quadratic Unconstrained Binary Optimization (QUBO) formulation.

The contents of this repository are part of the work titled:
## BPQ_RNA: A Thermodynamically Informed, Hybrid Quantum-Classical Framework for RNA 2D Structure Prediction Including Chemical Modifications

**Authors:** Nivedita Dutta, Quentin Vicens, and Liwen Shih

BPQ_RNA is a hybrid quantum-classical pipeline for predicting RNA secondary structures using a base-pair-level Quadratic Unconstrained Binary Optimization (QUBO) formulation. By mapping experimental Nearest Neighbor Database (NNDB) free energies directly onto the Hamiltonian, we bypass coarse-grained pre-assembly. This notebook implements the QUBO formulation, quantum optimization via QAOA (with randomized multistart initialization and multireplica sampling), and a classical maturation post-processing layer to resolve the energetic consequences of loops and dangling ends.

### Quick Start (Google Colab)

Click the badge below to run the BPQ_RNA pipeline directly in your browser:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/duttan710/BPQ_RNA/blob/main/BPQ_RNA_example.ipynb)

### Prerequisites & Hardware
* **Colab Runtime:** Standard T4 GPU (change runtime type)
* **Dependencies:** Pre-configured in the notebook's first setup cell (installs required quantum and bio-python packages automatically).

### Notebook Execution Flow
1. **Environment Initialization:** Imports NNDB parameters and quantum optimization libraries.
2. **Input Definition:** Pass RNA sequences including post-transcriptional modifications.
3. **QUBO Construction:** Maps NNDB free energy values directly onto the native base-pair Hamiltonian.
4. **QAOA Optimization:** Runs classical free energy-based baseline calculations vs. QAOA quantum optimization, tracking convergence.
5. **Maturation Layer:** Resolves energetic loop consequences and outputs the final secondary structure in dot-bracket format.
**Citation:** Dutta, N., Shih, L. A., Vicens, Q., BPQ_RNA: A Thermodynamically Informed, hybrid Quantum-Classical Framework for RNA 2D Structure Prediction Iincluding Chemical Modifications

## Free Energy Parameters

The experimentally derived Free energy parameters in efficiently utilizable formats are provided here: [Free Energy Parameters Gist](https://gist.github.com/duttan710/1429a1150dcd7d75fb5ca0cf29b92963/)

When utilizing the notebook or the integrated nearest neighbor free energy parameters, please also cite the following primary references:

1. Turner, D. H. & Mathews, D. H. (2009). NNDB: The nearest neighbor parameter database for predicting stability of nucleic acid secondary structure. *Nucleic Acids Research*, 38, D280-D282.
2. Mittal, A., Turner, D. H., & Mathews, D. H. (2024). NNDB: An Expanded Database of Nearest Neighbor Parameters for Predicting Stability of Nucleic Acid Secondary Structures. *Journal of Molecular Biology*, 168549.
3. Kierzek, E., Zhang, X., Watson, R.M. et al. (2022). Secondary structure prediction for RNA sequences including N6-methyladenosine. *Nat Commun*, 13, 1271.
