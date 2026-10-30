---
title: "Fluid Dynamics"
description: "Studying prolems across fluid dynamics, including data assimilation and Navier-Stokes alpha-models"
weight: -10
menu:
  sidebar:
    name: Fluid Dynamics
    identifier: fluid-dynamics
    parent: projects
# hero: bg.png
date: 2025-09-01T08:06:25+06:00
---

I connected with [Prof. Adam Larios at UNL](https://adamlarios.github.io/), who studies numerical partial differential equations (PDEs) and turbulence modeling. I studied materials across these areas, leading to work on the Navier–Stokes–Voigt equations (NSV), a regularized "alpha" model of the widely known Navier–Stokes equations (NSE). I earned a second award from the NASA Space Grant Consortium (for $6,400) to compare turbulence statistics of the 2D NSV and NSE. 

In [my REU on LCs]({{< ref "content/posts/projects/3D-LCs.md" >}}), I first recognized the discrepancy between mathematical results and information needed for real-world interpretation, a gap that data assimilation and related tools are designed to close. In my work with Prof. Larios, I have made concrete strides towards closing this gap by building my own second-order FEM (finite element method) solver for the NSE and NSV. I have reached high proficiency in a suite of advanced computational software libraries, including Firedrake, PETSc, and MPI. To facilitate massive high-resolution simulations, I co-authored a successful proposal securing 1,500,000 NSF ACCESS compute credits, enabling us to deploy my custom NSV solver across a high-performance computing cluster. 