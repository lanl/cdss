---
title: LANL Co-Design Summer School
layout: page
---

## What is the Co-Design Summer School?

The Los Alamos ISTI/ASC Co-Design Summer School was created to train future scientists to work on the kinds of interdisciplinary teams that are demanded by today’s scientific challenges. Launched in 2011, the summer school recruits top candidates in a range of fields spanning domain sciences, applied mathematics, computational and computer sciences, and computer architecture. Participants work together to solve a focused problem that is designed to build the skills needed to tackle the grand challenges of the future. Foremost among the skills on which we focus is the ability of students to work across disciplines with other team members, while employing their own unique expertise. This is the heart of Co-Design.

 Past summer school challenges have included problems in kinetic theory (Boltzmann Transport Equation), molecular dynamics, hydrodynamics (Adaptive Mesh Refinement), quantum molecular dynamics, astrophysics (core-collapse supernovae and neutron star mergers), and tabulated equations of state..  The summer school is hosted by the Applied Computer Science Group (CCS-7), lead by Linn Collins.

## What is Co-Design?

Co-Design is the social and technical equivalent of a multiple-constraint optimization problem.  The rapid evolution of computing architectures and the expanding space between specializations in domain science and computer architecture means that it is virtually impossible for a single individual to cover all of the skills needed to solve current-day computational science challenges.  Co-Design bridges this space through interactions between members of an interdisciplinary team.  With the right amount of overlap, team members can communicate with each other effectively to solve a problem.

## 2020 Co-Design Summer School Focus:

## Exploring Performance Portability of Flow and Reactive Transport in Environmental Applications to Water Quality

High Performance Computing platforms are increasingly built around heterogeneous designs built around different programming models. Lawrence Livermore National Laboratory and Oak Ridge Natioanl Laboratory have Sierra and Summit which are built around IBM and nVidia architectures. ORNL has further announced that their next machine, the exascale platform Frontier, wil lbe built around AMD architectures. Whereas Argonne National Laboratory has announced that its exascale platform, Aurora, will be provided by an Intel and Cray partnership.

Traditionally, scientific codes have been rewritten to take advantage of the native programming models of new platforms. With the expectation of vastly different platforms with wildly different programming models, this is no longer viable. To alleviate this issue, performance portability frameworks and models have been adopted. These models (e.g. Sandia National Laboratory's Kokkos and the Khronos Group's OpenCL) are designed to allow the same code to take advantage of architectures ranging from a manycore architecture to an nVidia or AMD GPU with minimal modifications. This allows application scientists to focus on how to better solve their problems rather than how to best use the latest leadership class facilities.

All of these performance portability frameworks are designed around interoperability. This means that the majority of a code can be written in a largely architecture agnostic manner while functions and kernels of interest can be adjusted on a per platform basis to take full advantage of the underlying hardware for all HPC platforms of interest.

This year's Co-Design Summer School will investigate and evaluate the trade-offs of performance portability frameworks in the context of the Amanzi code. (INSERT GENERAL DOMAIN FOCUS AREA SUMMARY). A quantitative and qualitative comparison of performance portability solutions and native programming models will improve overall knowledge of how to take advantage of the next generation of exascale supercomputers while improving our (GENERAL DOMAIN FOCUS AREA. Preferaly something where we are improving our knowledge of water quality?)

This school will serve to aid LANL's mission and explore the use of performance portability frameworks on exascale platforms within the context of the Amanzi code. Possible improvements include improved solver performance and ability to model rock weather fracturing and subsurface flows. This code is part of a wider LANL program aimed at open source watershed simulation.
