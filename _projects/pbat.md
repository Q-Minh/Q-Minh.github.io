---
title: "Physics Based Animation Toolkit"
excerpt: "Cross-platform C++ physically based simulation library with Python bindings for research scientists and engineers.<br><img src='/images/gpu.xpbd.bvh.gif'>"
collection: projects
---

Take a look at my open-source [cross-platform C++ physically based simulation library](https://github.com/Q-Minh/PhysicsBasedAnimationToolkit) (*PBAT*) with Python bindings for research scientists and engineers.

## Motivation

In research, in many cases, our bandwidth for designing algorithms is significantly higher than for implementing them. While end users of simulation tools can safely treat them as black boxes that take their inputs and generates the desired outputs, it is often the case that research scientists and engineers need to peel back the layers and examine the internals of such algorithms. 

*PBAT* aims to reveal these internal algorithmic building blocks that enable flexible composition of higher-level, application-specific simulation code, without sacrificing software implementation velocity.

## Features

### High-performance large scale non-linear hyperelasticity

*PBAT* provides state of the art time integrators for large scale simulation, including contact, such as [eXtended Position Based Dynamics](https://mmacklin.com/xpbd.pdf) (XPBD) and [Vertex Block Descent](https://graphics.cs.utah.edu/research/projects/vbd/vbd-siggraph2024.pdf) (VBD), which leverage the inherent massive parallelism of sparse local iterative solving schemes. The interested reader can expect awesome extensions/improvements to such algorithms that will push computational efficiency to even higher levels.

![gpu xpbd](/images/gpu.xpbd.bvh.gif)

### Real-time collision detection

Spatial and temporal coherency are exploited in *PBAT* to reduce the exponential cost of detecting geometric overlaps between primitives, i.e. collisions, by orders of magnitude. Effective collision culling paradigms such as [Sweep and Prune](https://en.wikipedia.org/wiki/Sweep_and_prune) and [Bounding Volume Hierarchies](https://en.wikipedia.org/wiki/Bounding_volume_hierarchy) are available on both CPU and GPU platforms.

![gpu broadphase](/images/gpu.broadphase.gif)

### Guaranteed intersection-free large deformation elastodynamics

*PBAT* is easily coupled to other existing scientific packages, such as [IPC Toolkit](https://ipctk.xyz/) to implement the game-changing [Incremental Potential Contact](https://ipc-sim.github.io/) method for guaranteed robust large deformation contact simulation.

![ipc bars](/images/ipc.bar.stacks.gif)

### Reduced subspace construction

Similarly, this coupling leverages Python's rich ecosystem of scientific computing tools (i.e. [scipy](https://scipy.org/), [pytorch](https://pytorch.org/), [jax](https://jax.readthedocs.io/en/latest/index.html)) to easily construct linear and non-linear subspaces for reduced order modeling.

![modal analysis](/images/beam.modes.gif)

### Finite element method (FEM) operators

A fundamental building block for spatial discretization in *PBAT* is the [finite element method](https://en.wikipedia.org/wiki/Finite_element_method), which *PBAT* abstracts behind operators and their matrix representations, which allows solving classical PDEs using numerical algorithms, applied to e.g. common geometry processing tasks such as harmonic interpolation, approximate geodesic distance computation and smoothing on curved domains.

![harmonic interpolation](/images/entei.harmonic.interpolation.order.2.png)
![heat geodesics](/images/metagross.heat.geodesics.png)
![mesh smoothing](/images/godzilla.diffusion.smoothing.gif)

