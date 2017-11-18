## [Concrete Dropout](https://arxiv.org/abs/1705.07832)

The replace discrete Bernoulli distribution in a traditional dropout with its continuous relaxation (Concrete distribution relaxation in the paper) to model the uncertain the a dropout neural network. This relasation can help us leverage low variance pathwise derivative estimator instead of the score function estimator. The variance analysis of different estimators can be found in Section 3 of [1]. 




## External Reference
[1]. Gal, Yarin. Uncertainty in deep learning. Diss. PhD thesis, University of Cambridge, 2016.