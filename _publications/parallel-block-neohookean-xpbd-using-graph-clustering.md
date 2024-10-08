---
title: "Parallel Block Neo-Hookean XPBD using Graph Clustering"
collection: publications
category: manuscripts
permalink: /publication/2024-Parallel-Block-Neo-Hookean-XPBD-using-Graph-Clustering
excerpt: "<img src='../images/parallel-block-neohookean-xpbd-bunny-colors.png'><br>**Best Paper Honorable Mention** at MIG 2022."
date: 2022-11-12
venue: 'Computers & Graphics'
slidesurl: 'https://Q-Minh.github.io/files/PBNH_XPBD_MIG.pdf'
paperurl: 'https://Q-Minh.github.io/files/PBNH_XPBD.pdf'
citation: 'Ton-That, Quoc-Minh, Paul G. Kry, and Sheldon Andrews. (2022, November). &quot;Parallel Block Neo-Hookean XPBD using Graph Clustering.&quot; <i>Computers & Graphics</i>. 110, 1-10.'
---

Video
------

[![Supplemental video](https://img.youtube.com/vi/MGgENtqyb7Q/0.jpg)](https://www.youtube.com/watch?v=MGgENtqyb7Q)

Short
------
Use our graph clustering technique for parallel execution of dense computational graphs to significantly speed up your workloads, especially on GPU hardware. Coupled with our blocked constraint formulation, we accelerate XPBD simulations by an order of magnitude.

Abstract
------
The eXtended Position Based Dynamics algorithm (XPBD) enables unified simulation of various materials from fluids to both elastic solids and stiff solids. In particular, finite element based neo-Hookean models can simulate near incompressible materials by means of a decoupled compliant constraint formulation. Due to XPBD’s reliance on local constraint projections in the solver loop, its computational nature lends itself to parallelization by means of graph coloring algorithms used to determine partitions of independent constraints which can be solved simultaneously. However, minimal graph coloring is bounded from below by the maximum valence of the finite element mesh, thus hindering parallelization opportunities. In this paper, we propose a novel graph clustering approach on the constraint graph which groups highly dependent constraints into supernodes. By applying graph coloring on the supernodal constraint graph, we are able to significantly reduce the number of partitions, thus enhancing parallelization of the solver. Furthermore, we accelerate convergence of the neo-Hookean XPBD solver by a coupled constraint formulation, resulting in enhanced stability and efficiency compared to previous approaches.

Awards
------
**Best Paper Honorable Mention** at MIG 2022. 
