---
title: "TAMU Summer School in PDEs"
description: "Learning more about mathematical modeling of partial differential equations (PDEs), particularly covering nonlinear elasticity"
weight: 5
menu:
  sidebar:
    name: TAMU Summer School in PDEs
    identifier: tamu-school
    parent: projects
hero: bg.png
date: 2026-05-30T08:06:25+06:00
---

I attended Texas A&M's annual [Undergraduate Summer School in Modeling and Simulation with PDEs](https://matthiasmaier.org/summerschool/). The first week, roughly 30 students and I recieved lectures from some of TAMU's best researchers: Dr. Matthias Meyer, Dr. Jean-Luc Guermond, and Dr. Andrea Bonito, along with visiting lecturer Dr. Diane Guignard from the University of Ottowa, Canada. I got the opportunity to review materials that I had already learned, including the finite element method (FEM), finite difference schemes, energy estimates, basic PDEs, and more. 

The second week, we really sank our teeth into modeling and simulating PDEs, breaking out into small groups of 3 students. My group was led by [Dr. Matthias Maier](https://matthiasmaier.org/). We simulated nonlinear elastic motion in Python, using the Navier-Lame equations. We started in 1D, comparing the nonlinear vs. linear equations for elasticity:
<video controls width="100%">
  <source src="./1d-viz.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
of course, after confirming convergence via the method of manufactured solutions.

Using some of my past experience modeling the Navier-Stokes equations, I made our 2D simulation from scratch, and got it to work midnight before the day of our presentation. My entire repository for the two weeks can be found [here](https://github.com/calvm32/TAMU_Summer_School).
<video controls width="100%">
  <source src="./2d1-2dview.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

I learned a lot about the PDEs governing different physical systems. Prior to this experience, I was only confident modeling fluid equations. After learning more about elasticity, expanding that knowledge to nonlinear elasticity, and coding a 2D solver from scratch, I feel a lot more confident applying my skills to study various physical phenomena. 