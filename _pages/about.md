---
permalink: /
author_profile: true
---

I am a mathematician at the Faculty of Mathematics, Informatics and Mechanics of the University of Warsaw. Starting from October 2026 I will hold there the position of Samuel Eilenberg Assistant Professor. Currently, I am a postdoc in a research project led by Błażej Miasojedow.

A recurring theme in my work is to understand complicated variational problems by identifying their effective structure: convexified energies, limiting models, optimal constants, or appropriate distances between mathematical objects.

## Elasticity and optimal design

One direction of my research concerns variational models for elastic structures and their optimal design. A typical problem is to minimize an energy of the form

\\[
\inf_{u,\chi}
\int_\Omega W(\nabla u(x),\chi(x))\,dx,
\\]

where \\(u\\) describes a deformation and \\(\chi\\) encodes the distribution of material. Such problems often lead to relaxation, convexification, and the emergence of effective energy densities.

<figure>
  <img src="/images/research/elasticity.png" alt="Elasticity and optimal design" style="max-width: 80%; display: block; margin: auto;">
  <figcaption style="text-align: center; font-size: 0.9em;">
    Example figure: an elastic membrane or an optimal material distribution.
  </figcaption>
</figure>

I am particularly interested in the analysis of reduced models for thin structures, including membrane and plate theories, and in the role played by convexity-type notions in deriving effective variational principles.

## Variational limits and relaxation

Many problems in the calculus of variations involve families of energies depending on a small parameter \\(\varepsilon\\). For instance, one may study energies of the form

\\[
E_\varepsilon(u)
=
\int_\Omega
f\left(x,\frac{x}{\varepsilon},\nabla u(x)\right)\,dx.
\\]

The goal is to understand the limiting behaviour of minimizers and minimum values as \\(\varepsilon \to 0\\). This naturally leads to \\(\Gamma\\)-convergence, homogenization, and relaxation.

<figure>
  <img src="/images/research/variational-limits.png" alt="Variational limits and relaxation" style="max-width: 80%; display: block; margin: auto;">
  <figcaption style="text-align: center; font-size: 0.9em;">
    Example figure: a sequence of variational problems converging to an effective limit.
  </figcaption>
</figure>

These questions are motivated by the fact that microscopic oscillations, singular perturbations, or nonconvex constraints may produce new macroscopic behaviour in the limit.

## Optimal transport and probability metrics

Another direction of my work concerns distances between probability measures and related sharp inequalities. A central example is the quadratic Wasserstein distance

\\[
W_2^2(\mu,\nu)
=
\inf_{\pi\in\Pi(\mu,\nu)}
\int_{\mathbb{R}^d\times\mathbb{R}^d}
|x-y|^2\,d\pi(x,y).
\\]

I am interested in comparing such distances with other probability metrics and in understanding the optimal constants and structural mechanisms behind these inequalities.

<figure>
  <img src="/images/research/optimal-transport.png" alt="Optimal transport" style="max-width: 80%; display: block; margin: auto;">
  <figcaption style="text-align: center; font-size: 0.9em;">
    Example figure: transport between two probability distributions.
  </figcaption>
</figure>

This line of research connects optimal transport, functional analysis, convexity, and measure theory.

## Selected publications

A full list of my publications and preprints is available on the [Publications page](/publications/).
