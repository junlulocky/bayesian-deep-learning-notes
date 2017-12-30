## [Conjugate-Computation Variational Inference : Converting Variational Inference in Non-Conjugate Models to Inferences in Conjugate Models](https://arxiv.org/abs/1703.04265)

The authors propose their method for variational inference computation for two classes of non-conjugate models. 
- The first class contains joint distribution for observed variables and hidden variables which can be split into a conjugate part and a non-conjugate part. For such models the proposed gradient steps can be expressed as a Bayesian inference in a conjugate model;
- The second class of models additionally allows conditionally-conjugate terms. For this model class, the proposed gradient steps can be written as a message passing algorithm where variational message-passing (VMP) or stochastic variational inference (SVI) is used for the conjugate part while stochastic gradients are employed for the rest.

The main concern of this paper is that the naive stochastic gradient descent in variational inferance may ignore the conjugate part of the lower bound (i.e. loss). The conjugate terms in the lower bound might have a **closed-form** expression and may not require any stochastic approximations. 

**Fun fact**: the authors provided a equivalent expression of gradient descent in equation (9) of the original paper.