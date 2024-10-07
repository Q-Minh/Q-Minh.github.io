---
title: "Generalized eXtended Finite Element Method for Deformable Cutting via Boolean Operations"
collection: publications
category: manuscripts
permalink: /publication/2024-Generalized-eXtended-Finite-Element-Method-for-Deformable-Cutting-via-Boolean-Operations
excerpt: "<img src='../images/gxfem-paper.png'><br>**Best Paper Award** at the 23rd ACM SIGGRAPH / Eurographics Symposium on Computer Animation (SCA2024)."
date: 2024-08-21
venue: 'Computer Graphics Forum'
slidesurl: 'https://Q-Minh.github.io/files/GXFEM_SCA.pptx'
paperurl: 'https://Q-Minh.github.io/files/GXFEM.pdf'
citation: 'Ton-That, Quoc-Minh, Paul G. Kry, and Sheldon Andrews. (2024, August). &quot;Generalized eXtended Finite Element Method for Deformable Cutting via Boolean Operations.&quot; <i>Computer Graphics Forum</i>. 43(8).'
---

Video
------

[![Supplemental video](https://img.youtube.com/vi/JiCJ2gy1Qxw/0.jpg)](https://www.youtube.com/watch?v=JiCJ2gy1Qxw)

Short
------
Discretize discontinuous functions on FEM meshes using our generalized XFEM (GXFEM) enrichment functions, which support multiple, complex and (self-)intersecting discontinuities. We apply GXFEM to cutting-enabled elastodynamic simulation.

Abstract
------
Traditional mesh-based methods for cutting deformable bodies rely on modifying the simulation mesh by deleting, duplicating, deforming or subdividing its elements. Unfortunately, such topological changes eventually lead to instability, reduced accuracy, or computational efficiency challenges. Hence, state of the art algorithms favor the extended finite element method (XFEM), which decouples the cut geometry from the simulation mesh, allowing for stable and accurate cuts at an additional computational cost that is local to the cut region. However, in the 3-dimensional setting, current XFEM frameworks are limited by the cutting configurations that they support. In particular, intersecting cuts are either prohibited or require sophisticated special treatment. Our work presents a general XFEM formulation that is applicable to the 1-, 2-, and 3-dimensional setting without sacrificing the desirable properties of the method. In particular, we propose a generalized enrichment which supports multiple intersecting cuts of various degrees of non-linearity by leveraging recent advances in robust mesh-Boolean technology. This novel strategy additionally enables analytic discontinuous integration schemes required to compute mass, force and elastic energy. We highlight the simplicity, expressivity and accuracy of our XFEM implementation across various scenarios in which intersecting cutting patterns are featured.

Awards
------
**Best Paper Award** at the 23rd ACM SIGGRAPH / Eurographics Symposium on Computer Animation (SCA '24). 