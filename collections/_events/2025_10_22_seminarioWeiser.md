---
layout: event_page
title: "Seminar - Integrating BDDC with Adaptive SDC Time Stepping and Lossy Compression for HPC Environments"
speaker: "Martin Weiser (Zuse Institute Berlin)"
standard_date: "22nd October 2025"
time: 11:30 CEST
where: "Aula Seminari -1 - Povo0 - Via Sommarive, 14 - Trento"
zoom_link: 
zoom_meeting_id: 
zoom_passcode: 
photo: /assets/images/events/seminar_cover.png
description: "Cardiac electrophysiology is described by PDEs of reaction-diffusion type with elliptic constraints, ranging from homogenized monodomain and bidomain models to extracellular-membrane-intracellular (EMI) models resolving the cardiac myocytes geometrically. Organ-scale s imulations and in particular large EMI simulations incur a high computational cost, since faithful excitation propagation requires fine meshes and small time steps. The locality of solution features calls for adaptive methods, but traditional mesh adaptivity, despite being effective in reducing the problem size,fails to provide speedup.
We present a novel low-overhead approach to adaptivity that works completely on the algebraic level and exploits shrinking correction support in spectral deferred correction (SDC) time stepping methods. We discuss its basic structure, its combination with balancing domain decomposition with constraints (BDDC) preconditioners, and its extension to second order finite element discretization using hierarchical elements and a hybrid multigrid-BDDC preconditioner.
We also consider lossy data compression for reducing the amount of data to be communicated in PDE solvers and preconditioners in particular. We discuss the transform coding framework, in-memory compression for overlapping Schwarz preconditioners for higher order FE as well as compressed inter-node communication in BDDC preconditioners. We present theoretical estimates and some numerical experience for efficiency improvements."

links: ""
---

**Contact person:** Simone Pezzuto.
