# Clustering in Contextual Bandits using Non-Parametrics and Particle Filtering-based Thompson Sampling

Code and report for EE392A (Undergraduate Project) at IIT Kanpur. All code is in Python, and requires numpy and pandas.

1. delicious_dynucb.ipynb - an implementation of the contextual bandit clustering algorithm in "Dynamic Clustering of Contextual Multi-Armed Bandits" (Nguyen & Lauw)
2. delicious_dynucb_dirichlet_process_means.ipynb - an non-parametric extension of the (1) using the DP-means algorithm in "Revisiting k-means: New Algorithms via Bayesian Nonparametrics" (Kulis & Jordan)
3. ictr_lda.ipynb - an implementation of "Online Interactive Collaborative Filtering Using Multi-Armed Bandit with Dependent Arms" (Wang et al.) considering the arms as known in advance (for comparison with (1) and (2)).
4. ictr_gmm.ipynb - an variation of (3) with GMM-style clustering.

### Data 

The data files may be downloaded as follows: "norm_matrix_ejml_full_delicious.csv" contains the PCA embeddings of the items aka bookmarks (based on the procedure in "Dynamic Clustering of Contextual Multi-Armed Bandits" (Nguyen & Lauw, CIKM 2014), taken from https://github.com/tronixplus/DYNUCB. Other files were taken from the links under "Delicious Bookmarks" at https://grouplens.org/datasets/hetrec-2011/. 

### Other references

1. "Efficient Thompson Sampling for Online Matrix-Factorization Recommendation" by Kawale et al. - the particle sampling-based Thompson sampling algorithm underlying (3) and (4).
