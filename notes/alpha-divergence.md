## [Dropout Inference in Bayesian Neural Networks with Alpha-divergences](https://arxiv.org/abs/1703.02914)

Dropout variational inference (VI) via KL divergence can severely underestimate model uncertainty or the model uncertainty is 'biased' (See [1] Section 3.3.2 or [2]). In short, by checking the equation of KL divergence, suppose the *q(w|.)* is the variational distribution and *p(w|.)* is the posterior distribution we want to use. The KL divergence will penalise *q(w)* for placing mass where *p(w|.)* has no or small mass and penalise less for not placing mass where *p(w|.)* has large mass. The author propose another objective function based on alpha-divergence that can overcome this problem.



## External Reference
[1]. Gal, Yarin. Uncertainty in deep learning. Diss. PhD thesis, University of Cambridge, 2016.
[2]. Turner, Richard E., and Maneesh Sahani. "Two problems with variational expectation maximisation for time-series models." Bayesian Time series models (2011): 115-138.