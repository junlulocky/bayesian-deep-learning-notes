## [Stochastic Variational Inference](https://arxiv.org/abs/1206.7051)

The authors claimed the SVI is scalable to large dataset and it approximates the posterior distribution in conjugate exponential-family models with **local** and **global** hidden variables.

[Assumption]: The Stochastic Variational Inference has extra assumption that the **complete conditionals** is from exponential family, where a complete conditional is the *conditional distribution of a hidden variable given the other **hidden variables** and the **observations***.

The variational distribution is assumed to be in the mean-field family and each factor of the hidden variables is assumed to be in the same exponential family as the associated complete conditional distributions, e.g.

[Prior distribution for hidden variables]: the prior distribution for the hidden variables has same for as its corresponding complete conditonals distribution. as shown in the equation (2) and equation (10) of the original paper. With these assumptions, we can optimize each coordinate in closed form rather than using coordinate ascent.

[The advantage of mean-field family]:
- the entropy term in ELBO decomposes;
- some other computations efficiencies in the coordinate update shown in equation (15) of the original paper;

[Stochastic]: The above VI is not efficient because it needs to go over all the data set. We can form **intermediate global parameters** using classical coordinate ascent updates where the sampled data point is **repeated N times**, i.e. use one data sample to represent the whole data set in one iteration; finally, we set the new global parameters to a **weighted average of the old estimate and the intermediate parameters**, in which case the author proved it is a form of **stochastic natural gradient**.



