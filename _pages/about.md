---
permalink: /
author_profile: true
---

I am an assistant professor of mathematics at the University of Warsaw, and my area of expertise lies at the intersection of two fields in the calculus of variations: optimal transport and optimal structural design. [(more info)](/aboutme/)

The goal of this webpage is sharing some of the research ideas that I have developed together with my collaborators.

I invite you to read my [papers](/publications/) for details and to [reach out](/contact/) with questions!


## 1. Kantorovich-Rubinstein duality of the second order

The celebrated K-R theorem states an equality between the 1-Wasserstein distance and a supremum over the set of 1-Lipschitz potentials. V.M. Zolotarev has brought the latter formulation to higher orders. For example, given two *centred* probabilities \\( \mu,\nu \in \mathcal{P}(\mathbb{R}^d)\\) of finite second moments, the 2-Zolotarev distance reads,

$$
	Z_2(\mu,\nu) := \sup \left\{ \int u\, d(\mu - \nu) \ : \  u\in C^{1,1}(\mathbb{R}^d), \ \ \mathrm{lip}(\nabla u) \leq 1  \ \right\}
$$

K-R duality tells us that  \\( Z_1 = W_1 \\) can be expressed via the Monge-Kantorovich optimal transport (OT) for the distance cost. In a joint <a href="https://arxiv.org/pdf/2412.00516" target="_blank" rel="noopener noreferrer">paper</a> with <a href="https://sites.google.com/site/gbouchitte/" target="_blank" rel="noopener noreferrer">Guy Bouchitté</a> we have found an OT formulation that underpins the second-order case. However, apart from the classical transport plan we also look for a vector-valued coupling,

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

The first consequence of our new K-R-type equality is a quantitative equivalence to 2-Wasserstein distance, which we have published in our <a href="https://arxiv.org/pdf/2511.00232" target="_blank" rel="noopener noreferrer">follow-up paper</a>,

$$
\frac{1}{4}\, W_2^2(\mu,\nu) \ \leq \ Z_2(\mu,\nu) \ \leq \ \frac{1}{2} \, (s_\mu + s_\nu)\, W_2(\mu,\nu)
$$

where \\(s_\mu, s_\nu\\) are the relevant standard deviations. The constants above are sharp.

Our second-order Kantorovich-Rubinstein duality is at the core of some of the topics that I expose below.



## 2. Optimal design of beam systems via OT

Still under construction!

<figure>
  <img src="/images/research/sig7.png" alt="Optimal transport" style="max-width: 70%; display: block; margin: auto;">
  <figcaption style="text-align: center; font-size: 0.9em;">
    An optimal beam system that transfer the weight of the slab to five columns.
  </figcaption>
</figure>




