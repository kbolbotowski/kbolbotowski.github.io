---
permalink: /
author_profile: true
---

I am an assistant professor of applied mathematics at the University of Warsaw [(more info)](/aboutme/), and my area of expertise lies at the intersection of two fields in the calculus of variations: optimal transport and optimal structural design. 

The goal of this webpage is to provide a concise overview of ideas I have developed together with my collaborators. I invite you to read my [papers](/publications/) for details and to [reach out](/contact/) with questions!

1. [Kantorovich--Rubinstein duality of the second order](#kantorovich-rubinstein-duality-second-order)
2. [Optimal design of beam systems via Optimal Transport](#optimal-design-of-beam-systems-via-ot)


<h2 id="kantorovich-rubinstein-duality-second-order" style="scroll-margin-top: 90px;">
  1. Kantorovich-Rubinstein duality of the second order
</h2>

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

<h2 id="optimal-design-of-beam-systems-via-ot" style="scroll-margin-top: 90px;">
  2. Optimal design of beam systems via Optimal Transport
</h2>

For two probability measures \\( \mu,\nu \in \mathcal{P}(\mathbb{R}^d)\\) consider the minimization problem with respect to a tensor-valued measure,

$$
\inf \left\{  \int  \Arrowvert\sigma\Arrowvert_{\mathrm{Sch},1} :  \sigma \in \mathcal{M}^b\bigl( \mathbb{R}^d;\mathbb{R}^{d \times d}_{\mathrm{sym}} \bigr), \ \ \mathrm{div}^2 \sigma = \mu-\nu \ \text{ in } \mathcal{D}'(\mathbb{R}^d)  \right\}
$$

Above \\(\Arrowvert\,\cdot\,\Arrowvert_{\mathrm{Sch},1} \\) is the <a href="https://en.wikipedia.org/wiki/Schatten_norm" target="_blank" rel="noopener noreferrer">Schatten 1-norm</a>, whereas \\(\mathrm{div}^2 \sigma = \sum_{i,j} \partial_{ij} \sigma_{ij}\\) is understood in the distributional sense. The infimum is finite and is achieved whenever \\(\mu\\) and \\(\nu\\) share the barycentre and have finite second moments.

<div style="display: flex; gap: 1.5em; justify-content: center; align-items: flex-start; flex-wrap: wrap;">

  <figure style="flex: 0 1 55%; margin: 0; text-align: center;">
    <img src="/images/research/Gatti.jpg"
         alt="Optimal beam system"
         style="width: 100%; display: block; margin: 0 auto;">
    <figcaption style="width: 100%; margin-top: 0.4em; text-align: center; font-size: 0.9em;">
      Gatti Wool Factory, picture by Pier Luigi Nervi, Rome 1953
    </figcaption>
  </figure>

</div>

In a plane, \\(d=2\\), the problem has a mechanical interpretation. Solution(s) \\( \sigma \\) is the <a href="https://en.wikipedia.org/wiki/Bending_of_plates" target="_blank" rel="noopener noreferrer">bending moment tensor</a> in the optimal (stiffest) ceiling subject to downward gravity forces \\(\mu \\) and equilbrated by the reaction forces \\( \nu \\) in the columns or walls. This design formulation builds upon the famous <a href="https://hal.science/file/index/docid/528973/filename/bouchitte-gangbo-seppecher.pdf" target="_blank" rel="noopener noreferrer">Michell problem</a> and can be viewed as its plate variant.





$$
\sigma^{x,y,z}(\xi) := |\xi-z|\,\Big(\tfrac{x-z}{|x-z|} \! \otimes \! \tfrac{x-z}{|x-z|} \mathcal{H}^1(\xi) {\, \mathbin{\Rule{0.13ex}{1.6ex}{0ex}\Rule{1.3ex}{0.13ex}{0ex}} \, } [x,z] -  \tfrac{y-z}{|y-z|} \! \otimes \! \tfrac{y-z}{|y-z|} \mathcal{H}^1(\xi) {\, \mathbin{\Rule{0.13ex}{1.6ex}{0ex}\Rule{1.3ex}{0.13ex}{0ex}} \, } [y,z] \Big)
$$

$$
\sigma(\xi) = \iiint \sigma^{x,y,\zeta(x,y)}(\xi) \, d\gamma(x,y), \qquad \text{where} \ \ \zeta = \frac{dq}{d\gamma}
$$

<div style="display: flex; gap: 1.5em; justify-content: center; align-items: flex-start; flex-wrap: wrap;">

  <figure style="flex: 0 1 45%; margin: 0; text-align: center;">
    <img src="/images/research/Lebvs5.png"
         alt="Data: Lebesgue meaures vs 5 Dirac deltas"
         style="width: 100%; display: block; margin: 0 auto;">
    <figcaption style="width: 100%; margin-top: 0.4em; text-align: center; font-size: 0.9em;">
      Data: Lebesgue meaures vs 5 Dirac deltas (slab's weight vs reaction forces in the columns)
    </figcaption>
  </figure>

  <figure style="flex: 0 1 45%; margin: 0; text-align: center;">
    <img src="/images/research/sig7.png"
         alt="Optimal beam system (discretized data)"
         style="width: 100%; display: block; margin: 0 auto;">
    <figcaption style="width: 100%; margin-top: 0.4em; text-align: center; font-size: 0.9em;">
      Optimal beam system (for discretized Lebesgue measure)
    </figcaption>
  </figure>

</div>



