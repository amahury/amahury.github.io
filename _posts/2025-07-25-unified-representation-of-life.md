---
title: "Review | Unified representation of Life’s basic properties by a 3-species Stochastic Cubic Autocatalytic Reaction-Diffusion system of equations"
date: 2025-07-25 00:00:00 -0400
categories: [Opinion]
tags: [review]
comments: true
toc: true 
math: true
pin: true 
mermaid: false
description: Reproduction, growth, development, homeostasis, metabolism, adaptation, evolution... we could go on and on and never find a complete list of characteristics that define life. However, another question is how to represent those properties using mathematical tools. Today we review an article by Muñuzuri and Pérez-Mercader whose objective is precisely that—to capture the key properties of life using a set of equations.
alpez:
  name: Amahury J. L. Diaz
  twitter: amahury0
---
### Introduction
The field of [Artificial Life](https://en.wikipedia.org/wiki/Artificial_life) (ALife) has long been driven by a dual imperative: the desire to simulate life-like phenomena and the ambition to realize them. Emerging from [cybernetics](https://en.wikipedia.org/wiki/Cybernetics), [theoretical biology](https://en.wikipedia.org/wiki/Mathematical_and_theoretical_biology), and the rise of [computer science](https://en.wikipedia.org/wiki/Computer_science), ALife has provided crucial insights into life’s basic principles by constructing artificial systems that mimic the behaviors of living organisms. These include [agent-based simulations](https://casci.binghamton.edu/publications/ps/agent_review.pdf), [robotic implementations](https://books.google.com/books?hl=en&lr=&id=pWsNJkdZ4tgC&oi=fnd&pg=PA3&dq=artificial+life+%2B+robotics&ots=88I0hZiQTD&sig=XXEiiEwDv0dKDqscLRXVz5inttA#v=onepage&q=artificial%20life%20%2B%20robotics&f=false), and [chemical prototypes](https://ieeexplore.ieee.org/abstract/document/6790776); all united by the common goal of abstracting life’s organization from its material instantiations.

However, as Howard Pattee forcefully argued in [_Simulations, Realizations, and Theories of Life_ (1989)](https://www.researchgate.net/profile/Howard-Pattee/publication/221586859_Simulations_Realizations_and_Theories_of_Life/links/0912f5017387295d4a000000/Simulations-Realizations-and-Theories-of-Life.pdf), a fundamental distinction must be made between simulation and realization. Simulations, no matter how precise, remain metaphorical representations. They “stand for” something else, never becoming that which they model. They presuppose a fixed set of rules and, therefore, cannot instantiate the genuine emergence, novelty, and semantic-pragmatic context that characterize living systems. Realizations, by contrast, are embodied and capable of generating unanticipated behavior by interacting with their environment. In living systems, symbolic information ([genotype](https://en.wikipedia.org/wiki/Genotype)) and material dynamics ([phenotype](https://en.wikipedia.org/wiki/Phenotype)) are irreducibly intertwined. This distinction is crucial for any theory that aspires to explain life beyond formal mimicry.

Despite this, simulations remain an indispensable heuristic tool. They enable us to explore conditions under which certain life-like properties could be realized, test theoretical unifications, and reveal the systemic interdependencies of life’s core features. It is precisely in this spirit that [Alberto P. Muñuzuri](https://cretus.usc.es/en/alberto-perez-munuzuri-eng/) and [Juan Pérez-Mercader](https://eps.harvard.edu/people/juan-perez-mercader/) propose [their model](https://www.sciencedirect.com/science/article/pii/S1571064522000185): a minimal, abstract, yet functionally expressive system of equations that aims to unify four properties shared by all known living systems, named information handling, metabolism, self-reproduction, and evolution. This effort constitutes a bold and rigorous attempt to model, at the level of chemical kinetics, a compact mathematical representation of what it means to be alive.

### Mathematical Representation of Life’s Properties
The authors begin with a sharp premise: all known forms of life, regardless of [complexity](https://en.wikipedia.org/wiki/Complexity), are open [non-equilibrium](https://en.wikipedia.org/wiki/Non-equilibrium_thermodynamics) chemical systems exhibiting four top-level properties. Rather than relying on the specificities of biochemical substrates, Muñuzuri and Pérez-Mercader seek an abstract and generalized representation of these properties using [reaction-diffusion equations](https://en.wikipedia.org/wiki/Reaction%E2%80%93diffusion_system); a well-established mathematical framework in [theoretical chemistry](https://en.wikipedia.org/wiki/Theoretical_chemistry) and [nonlinear dynamics](https://en.wikipedia.org/wiki/Nonlinear_system). 

They draw upon a rich lineage of theoretical contributions: [Turing’s reaction-diffusion model for morphogenesis](https://en.wikipedia.org/wiki/The_Chemical_Basis_of_Morphogenesis), [Sel’kov’s glycolysis equations](https://febs.onlinelibrary.wiley.com/doi/full/10.1111/j.1432-1033.1968.tb00175.x), [Prigogine’s non-equilibrium self-organization](https://archive.org/details/selforganization0000nico/page/n5/mode/2up), [Eigen’s hypercycles](https://en.wikipedia.org/wiki/Hypercycle_(chemistry)), [Gánti’s chemoton model](https://en.wikipedia.org/wiki/Chemoton), and the Artificial Life paradigms proposed by [Langton](https://en.wikipedia.org/wiki/Christopher_Langton) and [Adami](https://en.wikipedia.org/wiki/Chris_Adami). Yet, the novelty of their approach lies in integrating these diverse inspirations into a unified top-down framework, rather than assembling ad hoc modules for each property.

_Information handling_ is framed as a form of [chemical computation](https://www.cell.com/iscience/fulltext/S2589-0042(19)30285-8), requiring the system to support both linear and nonlinear transformations. The authors note that minimal computation can be chemically realized through automata such as switches and logic gates. However, rather than using large networks of explicitly defined gates, they invoke the power of nonlinear chemical reactions—especially sigmoid-like kinetics—as naturally embedded computational devices. These non-linearities, which emerge from quadratic and cubic terms in the kinetics, can instantiate switching behavior and support distributed information processing, particularly when coupled with diffusion in a spatially extended medium.

_Metabolism_, on the other hand, is understood as the maintenance of a critical free-energy gradient and the autonomous transformation of environmental input (or “food”) into internal system components. Here, the authors implement autocatalytic reactions such as $U + V \xrightarrow{\lambda} 2V$ and $U + 2V \xrightarrow{\lambda} 3V$, with the latter ensuring cubic non-linearity. These dynamics sustain the system far from equilibrium and embed a feedback mechanism through reaction rates, capturing the thermodynamic and kinetic essence of metabolism.

_Self-reproduction_ is introduced through the mechanism of [Turing instabilities](https://en.wikipedia.org/wiki/Reaction%E2%80%93diffusion_system#Two-component_reaction%E2%80%93diffusion_equations), which require at least two diffusing chemical species with differing diffusion constants and a cubic interaction term. Such instabilities generate spatial inhomogeneities (e.g., "domains") that act as protocell-like structures. When paired with oscillatory dynamics such as [Hopf bifurcations](https://en.wikipedia.org/wiki/Hopf_bifurcation), these domains exhibit periodic behavior analogous to the [Cell Division Cycle](https://en.wikipedia.org/wiki/Cell_cycle) (CDC). The authors emphasize that the same chemical species involved in self-replication must also contribute to information handling and metabolic control, ensuring internal coordination.

Finally, _evolution_ (both adaptive and non-adaptive) is modeled as the emergent behavior of a lattice of interconnected, locally autocatalytic nodes, or what the authors call “cell-like” domains. These nodes interact via diffusion and operate under stochastic perturbations, allowing for selection-like dynamics. Efficient configurations become more prevalent over time as noise-modified domains compete for resources. The structure, influenced by hypercycle theory, captures essential features of adaptation, mutation, and drift.

### Unification through the sCARD System
The conceptual cornerstone of the paper is the unification of all four life-properties into a single, parsimonious system of three coupled stochastic reaction-diffusion equations. These equations govern the dynamics of three abstract chemical species: the living system’s internal matter $V$, its nutrient or food $U$, and the waste product $C$. The reaction scheme is given by:

$$
\text{Reservoir}\xrightarrow{F} U;~~~ U+2V\xrightarrow{\lambda} 3V;~~~ V\xrightarrow{k} C
$$

Adding diffusion and noise terms yields the stochastic Cubic Autocatalytic Reaction-Diffusion (sCARD) model:

$$
\frac{\partial U}{\partial t} = -\lambda UV^2 + F(U_0 - U) + \eta_U + D_U \nabla^2 U \\
$$

$$
\frac{\partial V}{\partial t} = +\lambda UV^2 - (F+k)V + \eta_V + D_V \nabla^2 V
$$

$$
\frac{\partial C}{\partial t} = kV - FC + \eta_C + D_C \nabla^2 C
$$

This minimal model is expressive enough to support metabolism (via [autocatalysis](https://en.wikipedia.org/wiki/Autocatalysis)), information handling (via nonlinear switches), self-replication (via Turing-Hopf instabilities), and evolution (via stochastic lattice interactions and domain selection). The authors run simulations across various values of the parameters $F$ and $k$, revealing a rich phase space of behaviors, including cell-like domains that replicate and interact. 

[Figure 3](https://www.sciencedirect.com/science/article/pii/S1571064522000185#fg0030) of the paper depicts the [phase diagram](https://en.wikipedia.org/wiki/Phase_diagram) resulting from these simulations. Different behaviors, such as steady states, Turing spots and stripes, replicating domains, and chaotic mixes, occupy distinct parameter regions. Most notably, a “cell-like” zone emerges where domains form, replicate, and die, closely mimicking biological cells.

Physical observables are also extracted: the authors define a measure $\Phi(\textbf{r}, t) = \sum_{s=U, V, C} D_s \nabla^2 [s(\textbf{r}, t)]$. This function captures the divergence of diffusive flux and helps identify the emergent boundary of a domain, which is a mathematical analogue of a membrane. Additionally, they interpret the [negative entropy](https://en.wikipedia.org/wiki/Negentropy) of the domain as a proxy for its information content, tracking its dynamics through time to measure information flow and systemic organization.

### Results, Predictions, and Future Directions
The sCARD model leads to several striking results. Most notably, it reproduces key phases of the Cell Division Cycle (CDC): a domain grows, becomes unstable, and then divides into two daughter domains that inherit and carry on the cycle. This emergent behavior is not hard-coded but arises from the interaction of the model’s components, suggesting a fundamental link between [autocatalysis](https://en.wikipedia.org/wiki/Autocatalysis), [pattern formation](https://en.wikipedia.org/wiki/Pattern_formation), and [replication](https://en.wikipedia.org/wiki/Self-replication). 

Furthermore, the authors report signs of _primitive adaptation_. Stochastic simulations show that certain domains, those better suited to the fluctuating environment, come to dominate the population. These domains can also exhibit [_chemotactic behavior_](https://en.wikipedia.org/wiki/Chemotaxis), migrating toward resource-rich regions in the simulation field. At the population level, the system exhibits dynamics akin to the [Lotka-Volterra equations](https://en.wikipedia.org/wiki/Lotka%E2%80%93Volterra_equations), revealing predator-prey or competition-like interactions among multiple “cell-like” domains.

In essence, the authors demonstrate that three coupled equations describing abstract chemical species ($U$, $V$, and $C$) can serve as a minimal, unified model for life’s basic properties. While the model remains a simulation, it faithfully embodies the structure and dynamics necessary for a realization. The spatial lattice representation mimics the distributed nature of life’s organization, and the stochastic terms echo the inherent noise in molecular environments.

Looking ahead, the model offers several promising avenues. The authors suggest extending their simulations to 3D+time, linking their equations to concrete chemical instantiations, and comparing their approach to other synthetic life frameworks such as [Gánti’s chemoton](https://en.wikipedia.org/wiki/Chemoton), [Langton’s cellular automata](https://en.wikipedia.org/wiki/Langton%27s_loops), and [Adami’s AVIDA](https://en.wikipedia.org/wiki/Avida_(software)). They also point toward exploring [evolutionary transitions](https://www.nature.com/articles/374227a0), [emergent collectives](https://en.wikipedia.org/wiki/Collective_behavior), and [fitness landscapes](https://en.wikipedia.org/wiki/Fitness_landscape), using the model’s modularity to bridge theory and experiment.

Ultimately, Muñuzuri and Pérez-Mercader’s work stands as a bold theoretical synthesis: a minimalist framework that encodes the essence of life; not by mimicking its biochemical particulars, but by distilling its organizational logic into a coherent, extensible, and deeply physical formalism. Their contribution invites future exploration into the threshold where simulation may approach, though never become, realization. 

![Desktop View](/assets/img/fix/complexity-cat-newsletter.png){: .normal width="1200" height="630" }
