# MMT
 A Matlab Library for Multi-Task Learning

MMT is a Matlab toolbox implementing the multi-task Lasso models, including: (i) the Lasso; (ii) the standard multi-task Lasso, i.e. the group Lasso; (iii) the structured input-output multi-task Lasso, a.k.a. the two-graph guided multi-task Lasso proposed in [1]. The last case (iii) subsumes the special cases: tree-guided and the feature-graph guided multi-task Lasso. The core optimization algorithm for solving this model is developed in C to enhance greater computational efficiency. In particular, current scalability of the coefficient matrix that has been tested for MMT is 104*104! The structured input-output multi-task Lasso model is well-suited for addressing the expression quantitative trait loci (eQTL) mapping problems which are of the intrinsic high-dimensional nature. Details can be found in [1].

<strong>Input:</strong> an (n*p) regression matrix X, an (n*K) response matrix Y, an input graph G1 on X and an output graph G2 on Y, representing the prior structures on the columns of X and Y, respectively, regularization parameters λ1 and λ2 for the two prior graphs, and an (optional) initial guess of the coefficient matrix.

<strong>Output:</strong> a (p*K) estimated sparse coefficient matrix B.

<strong>Usage:</strong> please refer to the file ./doc/mmt_user_manual.pdf

<strong>References:</strong>

[1] A two-graph guided multi-task Lasso approach for eQTL mapping. Xiaohui Chen, Xinghua Shi, Xing Xu, Zhiyong Wang, Ryan E. Mills, Charles Lee, Jinbo Xu. (2012) International Conference on Artificial Intelligence and Statistics (AISTATS'12).
