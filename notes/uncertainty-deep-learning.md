## [Uncertainty in Deep Learning](https://pdfs.semanticscholar.org/a6af/62389c6655770c624e2fa3f3ad6dc26bf77e.pdf)

Out of distribution test data: If the model has been train on the dog dataset and when we feed the model with cat pictures, the model would give random outputs.Bayesian deep learning can be leveraged to provide the information of uncertainty in the model outputs. In general, two kinds of uncertaincy measurement can be considered: 
- **Epistemic uncertainty**: a large number of model parameter can explain the training data very well, i.e. we are uncertain which parameter is 'true'; also several model structures can also explain the training data very well, we are unsure about the model structure.
- **Aleatoric uncertainty**: the observed data can be noisy.

Combining the epistemic uncertainty and aleatoric uncertainty together, we can induce **predictive uncertainty** normally.

Deep learning in general does point estimate so that it does not provide such uncertainty information. 

- Bayesian neural networks: model uncertainty in neural networks can be obtained by plaing distribitions over the weights. 

Stochastic regularisation techniques (SRTs) are used to model the uncertainty in neural networks. Popular SRTs include dropout, multiplicative Gaussian noise, dropConnect and many others. 

- Drawback of the SRTs: we need to repeate several times for this process to obtain the uncertainty.

### Bayesian Modelling
Putting prior distribution over the parameters which represents our prior beliefs over these parameters and observe the training data, we can capture the more likely parameters and less likely parameters. 

To predict the new data points, we need to marginalise w.r.t the parameters in the prior distribution. If the likelihood is conjugate to the prior distribution, then it is analytically tractable; otherwise, we need some approximate inference methods such as variational inference etc. Variation infernece replces Bayesian modelling marginalisation with optimisation, i.e. it replaces the integral in Bayesian modelling with derivative calculation in optimisation. 




