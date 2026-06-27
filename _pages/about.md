---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

---

permalink: /
title: "Karol Bołbotowski"
author_profile: true
--------------------

I am a mathematician working in the calculus of variations, optimal design, elasticity, and related questions in analysis. My research is concerned with variational models arising from mechanics and geometry, with particular emphasis on sharp asymptotic descriptions, relaxation, and the structure of optimal configurations.

I am currently interested in problems where analytical methods interact with models from continuum mechanics, shape optimization, and optimal transport. A recurring theme in my work is to understand how complicated microscopic or geometric constraints can be replaced by effective variational principles.

## Elasticity and optimal design

One direction of my research concerns variational models for elastic structures and their optimal design. A typical problem is to minimize an energy functional of the form

[
\inf_{u,\chi} \int_\Omega W(\nabla u(x),\chi(x)),dx,
]

where (u) describes a deformation and (\chi) encodes the distribution of material. Such problems often lead to relaxation, convexification, and the emergence of effective energy densities.

<figure>
  <img src="/images/research/elastic-membrane.png" alt="Elastic membrane example" style="max-width: 80%; display: block; margin: auto;">
  <figcaption style="text-align: center; font-size: 0.9em;">
    Example figure: an elastic membrane or an optimal material distribution.
  </figcaption>
</figure>

A particular interest is the derivation and analysis of reduced models for thin structures, including membrane and plate theories. These questions are closely connected with quasiconvexity, lower semicontinuity, and the fine structure of minimizing sequences.

## Variational limits and relaxation

Many problems in the calculus of variations involve families of energies depending on a small parameter, for example

[
E_\varepsilon(u) = \int_\Omega f\left(x,\frac{x}{\varepsilon},\nabla u(x)\right),dx.
]

One wants to understand the limiting behaviour of minimizers and minimum values as (\varepsilon \to 0). This naturally leads to notions such as (\Gamma)-convergence, homogenization, and relaxation.

<figure>
  <img src="/images/research/variational-limit.png" alt="Variational limit illustration" style="max-width: 80%; display: block; margin: auto;">
  <figcaption style="text-align: center; font-size: 0.9em;">
    Example figure: a sequence of variational problems converging to an effective limit.
  </figcaption>
</figure>

The goal is often to replace a singular or highly oscillatory model by a limiting energy which is analytically tractable but still retains the essential features of the original problem.

## Optimal transport and probability metrics

Another research direction concerns distances between probability measures, especially those connected with optimal transport. For example, the quadratic Wasserstein distance is given by

[
W_2^2(\mu,\nu)
==============

\inf_{\pi \in \Pi(\mu,\nu)}
\int_{\mathbb{R}^d \times \mathbb{R}^d}
|x-y|^2,d\pi(x,y).
]

I am interested in inequalities between probability metrics and their role in analysis, approximation, and limit theorems.

<figure>
  <img src="/images/research/optimal-transport.png" alt="Optimal transport illustration" style="max-width: 80%; display: block; margin: auto;">
  <figcaption style="text-align: center; font-size: 0.9em;">
    Example figure: transport between two probability distributions.
  </figcaption>
</figure>

These questions often combine tools from functional analysis, convexity, and measure theory.

## Selected publications

A full list of publications is available [here](/publications/).

