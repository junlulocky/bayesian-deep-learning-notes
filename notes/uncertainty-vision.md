## [What Uncertainties Do We Need in Bayesian Deep Learning for Computer Vision?](https://arxiv.org/abs/1703.04977)

This paper is a complementary material for introduction of different types of uncertainty in deep learning to [1]. 
- **Epistemic uncertainty**: a large number of model parameter can explain the training data very well, i.e. we are uncertain which parameter is 'true'; also several model structures can also explain the training data very well, we are unsure about the model structure.
- **Aleatoric uncertainty**: the observed data can be noisy.

Aleatoric uncertainty can further be categorized into
- **Homoscedastic** uncertainty: uncertainty which stays constant for different inputs
- **Heteroscedastic** uncertainty: Heteroscedastic uncertainty depends on the inputs to the model, with some inputs potentially having more noisy outputs than others.

The paper further introduces how to model these uncertainty: 
- Epistemic uncertainty is modeled by placing a **prior distribution** over a model’s weights, and then trying to capture how much these weights vary given some data. Such method in neural networks is referred as Bayesian neural networks (BNN);
- Aleatoric uncertainty is modeled by placing a distribution over the output of the model, e.g Gaussian random noise on the output.

Most importatly, the authors showed how to combine Aleatoric and Epistemic uncertainty in one model.

## External Reference
[1]. Gal, Yarin. Uncertainty in deep learning. Diss. PhD thesis, University of Cambridge, 2016.
