---
permalink: /
author_profile: true
---

I am a mathematician at the Faculty of Mathematics, Informatics and Mechanics of the University of Warsaw. More info about me can be found [here](/aboutme/). 

Below I present some of the research themes in calculus of variations that I have developed with my collaborators. Feel free to [contact](/contact/) me with questions!


## Topic #1: Kantorovich-Rubinstein duality beyond the first order

Famouosly, the classical K-R duality states an equality between the 1-Wasserstein distance (expressed by the Monge-Kantorovich optimal transport) and a supremum over the set of 1-Lipschitz potentials. V.M. Zolotarev has brought the latter formulation to higher orders. For example, given two probabilities \\( \mu,\nu \in \mathcal{P}(\mathbb{R}^d)\\) of finite second moments, the second Zolotarev distance reads,

$$
	Z_2(\mu,\nu) = \sup \left\{ \int u\, d(\mu - \nu) \ : \  u\in C^{1,1}(\mathbb{R}^d), \ \ \mathrm{lip}(\nabla u) \leq 1  \ \right\},
$$

while \\( Z_1 = W_1 \\). Note that finiteness of \\(Z_2\\) requires a match of the barycentres of the two probabilities. 

$$
	Z_2(\mu,\nu) = \! \! \! \! \min_{\substack{\gamma \in\mathcal{P}(\mathbb{R}^d \times \mathbb{R}^d) \\\ q \in \mathcal{M}( \mathbb{R}^d \times \mathbb{R}^d;\mathbb{R}^d) }} \! \! \left\{ \iint \frac{1}{2}\Big(\left|\tfrac{dq}{d\gamma}(x,y)-x\right|^2 + \left|\tfrac{dq}{d\gamma}(x,y)-y\right|^2 \Big) d\gamma(x,y) \ : \ \begin{array}{l}
		\pi_1^\# \gamma = \mu, \\
		\pi_2^\# \gamma=\nu,
	\end{array} \ \ \begin{array}{l}
		\pi_1^\#  q = x \mu \\
		\pi_2^\#  q = y \nu
	\end{array}
	 \ \right\}
$$

$$
\frac{1}{4}\, W_2^2(\mu,\nu) \ \leq \ Z_2(\mu,\nu) \ \leq \ \frac{1}{2} \, (\sigma_\mu + \sigma_\nu)\, W_2(\mu,\nu)
$$

<figure>
  <img src="/images/research/sig7.png" alt="Optimal transport" style="max-width: 30%; display: block; margin: auto;">
  <figcaption style="text-align: center; font-size: 0.9em;">
    Example figure: transport between two probability distributions.
  </figcaption>
</figure>


## Selected publications

A full list of my publications and preprints is available on the [Publications page](/publications/).

