---
title: "Centre Inria de l'université de Bordeaux | Post-Doctoral Research Visit on inferring structure in complex systems"
date: 2026-08-15 00:00:00 -0400
categories: [Community]
tags: [job, postdoc]
comments: false
toc: true
math: false
mermaid: false
description: The Centre Inria de l'université de Bordeaux offers a two-year post-doctoral position focusing on inferring structure in complex systems.
alpez:
  name: Amahury J. L. Diaz
  twitter: amahury0
---
### Context
Traditionally physical science operates under two fundamental assumptions: one, that the universe may be reduced to a set of consistent parts and fundamental laws that govern their behavior; two, that the universe and its phenomena may then be reconstructed from this set of fundamental laws. And yet many natural phenomena possess emergent properties that are difficult or even mathematically impossible to deduce even from a complete microscopic description [1, 2].The existence of irreducibly complex systems presents a challenge: to build a science of model discovery beyond the traditional reductionist-constructionist paradigm. 

There are important questions: what is the meaning of structure, divorced from a domain-specific physical context? Can we mathematically define it and detect it? How does one build a consistent mathematical language to describe things as disparate as bird flocking behavior and the formation of galaxies? Why do patterns emerge in physical systems over time? Can we predict when ‘something new’ will emerge, and can we detect it once it has emerged [3]? What counts as something new?

At Inria we take a dual-pronged approach of tackling both these questions on both a theoretical level, by developing the aforementioned mathematical tools, and on a practical level, by applying these tools to real world systems in collaboration with domain scientists.

Our primary focus is causal state and structure discovery from time series. Our method takes in time series of observations and returns a set of inferred causal states of the system—sets of predictively equivalent observations—with an interpretable geometry [4, 5]. This is a stochastic parallel to deterministic attractor reconstruction in nonlinear dynamics. The inferred causal state set can be analyzed for insights into the intrinsic complexity and mechanistic drivers of the underlying system. When paired with inference of the governing equations of motion, it can also be used as the state set of an inherently interpretable, optimally predictive model [6, 7].

We are developing a software package based on existing code that implements our inference algorithm using kernel embedding of conditional probability distributions [cite]. The algorithm takes in arbitrary time series (including observations from multiple sources or heterogeneous data) and returns the inferred causal state set in the form of similarity matrices, which are then dimension reduced for visualization and analysis [8]. This software package is to be disseminated to the public. It is also to be used in the framework of a partnership between Inria and Inrae to improve modeling of carbon flux dynamics in ecosystems.

 

[1] P.W. Anderson. More is different. Science, 177(4047):393–396, August 1972.

[2] M. Gu, C. Weedbrook, A. Perales, and M. Nielsen. More really is different. Physica D, 238(9-10):835–839, May 2009.

[3] James P. Crutchfield. The calculi of emergence: Computation, dynamics, and induction. Physica D, 75:11–54, 1994.

[4] Nicolas Brodu and James P. Crutchfield. Discovering causal structure with reproducing-kernel Hilbert space \epsilon-machines. Chaos: An Interdisciplinary Journal of Nonlinear Science, 32(2):023103, 02 2022.

[5] Samuel P. Loomis and James P. Crutchfield. Topology, convergence, and reconstruction of predictive states. Physica D: Nonlinear Phenomena, 445:133621, 2023

[6] C. R. Shalizi. Causal Architecture, Complexity and Self-Organization in Time Series and Cellular Automata. PhD thesis, University of Wisconsin, Madison, Wisconsin, 2001.

[7] S.L. Brunton, J.L. Proctor, & J.N. Kutz, Discovering governing equations from data by sparse identification of nonlinear dynamical systems, Proc. Natl. Acad. Sci. U.S.A. 113 (15) 3932-3937, https://doi.org/10.1073/pnas.1517384113 (2016).

[8] Alexandra M. Jurgens, Nicolas Brodu; Inferring kernel -machines: Discovering structure in complex systems. Chaos 1 March 2025; 35 (3): 033162. https://doi.org/10.1063/5.0242981 

### Assignment
With the help of Alexandra Jurgens (Inria) and a to-be-recruited engineer (Inria) the recruited person will work to further use their knowledge of stochastic processes and information theory to develop a mathematical definition and inference method for equations of motion of the causal states on the inferred causal structures. These equations of motion are, generically, stochastic differential equations and may be difficult to infer, even if they are relatively simple to define mathematically. Success in this project will allow the inferred causal state set to be paired with the equations of motion to form a predictive model, closing the inference loop. As a follow up to this, the postdoc will define and develop calculation methods for information theoretic measures (such as the Shannon entropy rate) that describe the predictive model. A secondary goal of the post doc is to investigate the role that kernel choice plays in causal structure inference by testing the dependence of the aforementioned information theoretic measures on kernel choice.

The principal place of work will be the Inria center at the University of Bordeaux. 

Responsibilities: The person recruited will be responsible for studying the governing equations of motion of an inferred dynamical attractor. They will also be asked to write and present this research in scientific journals. 

### Main activities
- Defining flows of probabilistic states on an inferred attractor structure. These flows are, generically, described by stochastic differential equations
- Work with a team towards an implementable algorithm for the inference of these equations (this may only be possible in special cases–which cases is a question of interest)
- Define and develop algorithms for information theoretic measures descriptive of the inferred attractor and the equations of motion
- Write mathematical reports and scientific articles on the above topics

Additional activities:
- Present progress of ongoing work to colleagues and partners
- Discuss with scientific collaborators

### Skills
Technical skills: The major activity of this postdoc requires skills in stochastic processes, predictive modeling, and information theory as well as interest in complexity, geometry, and topology. There is an expectation of fluency in scientific coding to translate mathematical work into actionable algorithms for implementation in the team’s software package, but this will be done in tandem with a full-time software engineer.

Interdisciplinary skills: Ability to communicate with colleagues from computer science, physics, and ecology will be necessary. In particular, interest in physics—especially in complexity, chaos, information theory, and/or stochastic thermodynamics—or nonlinear dynamics would be an advantage. 

Languages: Candidates must be at ease in scientific English and eager to publish their results in scientific journals. The team uses English.

### Benefits package
- Subsidized meals
- Partial reimbursement of public transport costs
- Possibility of teleworking and flexible organization of working hours
- Professional equipment available (videoconferencing, loan of computer equipment, etc.)
- Social, cultural and sports events and activities
- Access to vocational training
- Social security coverage

Application and more details: [https://recrutement.inria.fr/public/classic/en/offres/2026-10198](https://recrutement.inria.fr/public/classic/en/offres/2026-10198)

![Desktop View](/assets/img/fix/complexity-cat-newsletter.png){: .normal width="1200" height="630" }
