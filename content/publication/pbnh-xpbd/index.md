---
title: "Parallel Block Neo-Hookean XPBD using Graph Clustering"
authors:
- admin
- Paul G. Kry
- Sheldon Andrews
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2022-11-12T00:00:00Z"
doi: "https://doi.org/10.1016/j.cag.2022.10.009"

# Schedule page publish date (NOT publication's date).
publishDate: "2024-10-08T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*Computers & Graphics, 110*, 1-10"
publication_short: ""

abstract: The eXtended Position Based Dynamics algorithm (XPBD) enables unified simulation of various materials from fluids to both elastic solids and stiff solids. In particular, finite element based neo-Hookean models can simulate near incompressible materials by means of a decoupled compliant constraint formulation. Due to XPBD’s reliance on local constraint projections in the solver loop, its computational nature lends itself to parallelization by means of graph coloring algorithms used to determine partitions of independent constraints which can be solved simultaneously. However, minimal graph coloring is bounded from below by the maximum valence of the finite element mesh, thus hindering parallelization opportunities. In this paper, we propose a novel graph clustering approach on the constraint graph which groups highly dependent constraints into supernodes. By applying graph coloring on the supernodal constraint graph, we are able to significantly reduce the number of partitions, thus enhancing parallelization of the solver. Furthermore, we accelerate convergence of the neo-Hookean XPBD solver by a coupled constraint formulation, resulting in enhanced stability and efficiency compared to previous approaches.

# Summary. An optional shortened abstract.
summary: |
  Best Paper honourable mention at the 15th annual ACM/SIGGRAPH conference on Motion, Interaction and Games (MIG 2022).

tags:
- Publications
featured: true

# links:
# - name: ""
#   url: ""
url_pdf: http://profs.etsmtl.ca/sandrews/pdf/xpbdBlockNeo_MIG22_preprint.pdf
url_code: 'https://github.com/Q-Minh/PhysicsBasedAnimationToolkit'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'http://profs.etsmtl.ca/sandrews/slides/MIG22_Parallel_block_neohookean.pdf'
url_source: ''
url_video: 'https://drive.google.com/file/d/1op_UiIvcrV6cvTvdxrXJafIVXg5Mwgqz/view?usp=sharing'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

{{< youtube MGgENtqyb7Q >}}

<span style="color:red"><b>Best Paper</b></span> honourable mention at the 15th annual ACM/SIGGRAPH conference on Motion, Interaction and Games (MIG 2022).

## Cite

```bib
@article{blockNeo22_preprint,
    author = {Ton-That, Quoc-Minh and Kry, Paul G. and Andrews, Sheldon},
    title = {Parallel Block Neo-Hookean XPBD using Graph Clustering},
    journal = {Computers & Graphics},
    volume = {110}, 
    pages = {1--10},
    year = {2023},
    doi = {10.1016/j.cag.2022.10.009}
}
```

