## [Uncertainty in Deep Learning](https://pdfs.semanticscholar.org/a6af/62389c6655770c624e2fa3f3ad6dc26bf77e.pdf)

Out of distribution test data: If the model has been train on the dog dataset and when we feed the model with cat pictures, the model would give random outputs.Bayesian deep learning can be leveraged to provide the information of uncertainty in the model outputs. In general, two kinds of uncertaincy measurement can be considered: 
- Epistemic uncertainty: a large number of model parameter can explain the training data very well, i.e. we are uncertain which parameter is 'true'; also several model structures can also explain the training data very well, we are unsure about the model structure.
- Aleatoric uncertainty: the observed data can be noisy.

Combining the epistemic uncertainty and aleatoric uncertainty together, we can induce *predictive uncertainty* normally.
