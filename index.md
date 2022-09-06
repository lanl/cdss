---
title: LANL Co-Design Summer School
layout: page
---

## What is the Co-Design Summer School?

The Los Alamos National Laboratory Co-Design Summer School was created to train future scientists to work on the kinds of interdisciplinary teams that are demanded by today’s scientific challenges. Launched in 2011, the summer school recruits top candidates in a range of fields spanning domain sciences, applied mathematics, computational and computer sciences, and computer architecture. Participants work together to solve a focused problem that is designed to build the skills needed to tackle the grand challenges of the future. Foremost among the skills on which we focus is the ability of students to work across disciplines with other team members, while employing their own unique expertise. This is the heart of Co-Design.

Past summer school challenges have included problems in kinetic theory (Boltzmann Transport Equation), molecular dynamics, hydrodynamics (Adaptive Mesh Refinement), quantum molecular dynamics, astrophysics (core-collapse supernovae and neutron star mergers), and tabulated equations of state. The summer school is hosted by the Applied Computer Science Group (CCS-7), led by Christoph Junghans.

## What is Co-Design?

Co-Design is the social and technical equivalent of a multiple-constraint optimization problem. The rapid evolution of computing architectures and the expanding space between specializations in domain science and computer architecture means that it is virtually impossible for a single individual to cover all of the skills needed to solve current-day computational science challenges. Co-Design bridges this space through interactions between members of an interdisciplinary team. With the right amount of overlap, team members can communicate with each other effectively to solve a problem.

## 2023 Co-Design Summer School Focus:

## Simulation of burn front type Ia supernova at scale 


Los Alamos National Laboratory will be hosting a new supercomputer, Venado, in the Spring of 2023. This machine will embed the new Nvidia achitectures, Grace and Grace Hopper Superchips, on top of the HPE Shasta system. This CPU and GPU coupled architecture is expected to give an immediate performance boost to a wide range of HPC applications.

In order to perform on such a machine, the applications need to harness the computational power of thousands of nodes and perform efficiently on different types of architectures such as CPU (x86, ARM), GPGPU (Nvidia, AMD) or future platforms. For the latter, multiple solutions now exist providing their own paradigm of data representation and the ability to target these different platforms. Programming models, such as Kokkos or Raja, provide such a solution and avoid the cost of rewriting the code to run on different architectures. 


Type Ia supernovae are powerful cosmological events that are actively studied in astrophysics. Although there is a considerable amount of studies on Type Ia supernovae e.g. its progenitors and observational signatures, the explosion mechanism is still a topic of discussion. One of the most popular mechanisms is called the single-degenerate scenario. In this case, the white dwarf gains mass from its companion and starts to contract, increasing its temperature and density. 
Once the mass approaches the Chandrasekhar limit, a burning front is formed inside of the star, where carbon and oxygen are fused into intermediate mass and iron-group elements. These are the building blocks of all planets and the life on them. The burning front starts out originally as a subsonic deflagration, but may go through a deflagration-to-detonation transition to trigger a supersonic detonation, which can consume the rest of the white dwarf. 

White dwarfs with a helium layer on their surface can undergo another type of explosion. In the sub-Chandrasekhar scenario the accretion of material from a companion star triggers a detonation in the helium layer.
This wraps around the white dwarf and sends shock waves to the core, triggering a carbon--oxygen detonation.
To capture the energy of the reaction front and the elements produced in nucleosynthesis, the hydrodynamics code needs to include a nuclear reaction network. An efficient implementation and coupling of the network will allow us to run with a large number of species, which is the basis for providing data to modelers creating artificial spectra using radiative transfer simulations. These spectra give a direct connection to observations.

The goal for the 2023 Co-Design Summer School will be to simulate the burn front of Type Ia supernovae at a large scale platform like Venado, Crossroads or El Capitan.
The team of students will have to tackle several topics in a Co-Design manner to reach this goal. The computer scientists, applied mathematicians and physicists will work together in Co-Design to add the support for reaction network, efficient load balancing, optimize the code and check the convergence properties.
As a foundation, the students will use [Parthenon-Hydro](https://github.com/pgrete/parthenon-hydro) which is based on [Parthenon](https://github.com/lanl/parthenon).  Parthenon is a performance portable block-structured adaptive mesh refinement framework. It adopts Kokkos programming model which allows developers to write performance portable applications targeting all major HPC platforms. 
The Parthenon code will provide a new feature, Sparsity on the Block, which will allow the representation of hollow regions of the domain without allocating memory.
This feature coupled with the expertise and optimizations on the Nvidia H100 architecture will be the key to reach performances for the burn front simulations at scale. 

LA-UR-22-29148
