---
title: "* Generalized eXtended Finite Element Method for Deformable Cutting via Boolean Operations"
authors:
- admin
- Paul G. Kry
- Sheldon Andrews
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2024-08-21T00:00:00Z"
doi: "https://doi.org/10.1111/cgf.15184"

# Schedule page publish date (NOT publication's date).
publishDate: "2024-10-08T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*Computer Graphics Forum, 43*(8)"
publication_short: ""

abstract: Traditional mesh-based methods for cutting deformable bodies rely on modifying the simulation mesh by deleting, duplicating, deforming or subdividing its elements. Unfortunately, such topological changes eventually lead to instability, reduced accuracy, or computational efficiency challenges. Hence, state of the art algorithms favor the extended finite element method (XFEM), which decouples the cut geometry from the simulation mesh, allowing for stable and accurate cuts at an additional computational cost that is local to the cut region. However, in the 3-dimensional setting, current XFEM frameworks are limited by the cutting configurations that they support. In particular, intersecting cuts are either prohibited or require sophisticated special treatment. Our work presents a general XFEM formulation that is applicable to the 1-, 2-, and 3-dimensional setting without sacrificing the desirable properties of the method. In particular, we propose a generalized enrichment which supports multiple intersecting cuts of various degrees of non-linearity by leveraging recent advances in robust mesh-Boolean technology. This novel strategy additionally enables analytic discontinuous integration schemes required to compute mass, force and elastic energy. We highlight the simplicity, expressivity and accuracy of our XFEM implementation across various scenarios in which intersecting cutting patterns are featured.

# Summary. An optional shortened abstract.
summary: Discretize discontinuous functions on FEM meshes using our generalized XFEM, which supports multiple, complex and (self-)intersecting discontinuities.

tags:
- Publications
featured: true

# links:
# - name: ""
#   url: ""
url_pdf: http://profs.etsmtl.ca/sandrews/pdf/SCA24_cutting.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'http://profs.etsmtl.ca/sandrews/slides/GXFEM_SCA24.pptx'
url_source: ''
url_video: 'https://drive.google.com/file/d/1RBjv7mK-1c6A-3KVVBBuow963CBWRvGO/view?usp=drive_link'

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

{{< youtube JiCJ2gy1Qxw >}}

<span style="color:red"><b>Best Paper</b></span> award at the 23rd ACM SIGGRAPH / Eurographics Symposium on Computer Animation (SCA '24).

### Cite

```bib
@article{xfemCutting2024,
    author = {Ton-That, Quoc-Minh and Kry, Paul G. and Andrews, Sheldon},
    title = {Generalized eXtended Finite Element Method for Deformable Cutting via Boolean Operations},
    journal = {Computer Graphics Forum},
    volume = {43},
    number = {8},
    year = {2024},
    numpages = {13},
    doi = {10.1111/cgf.15184}
}
```