---
# Leave the homepage title empty to use the site title
title: ""
date: 2024-10-11
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/CV.pdf
    design:
      background:
        image:
          # Add your image background to `assets/media/`.
          filename: animated-shapes.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 Research'
      subtitle: ''
      text: |-
        I leverage massively parallel computing techniques via GPGPU programming, graph processing, efficient large-scale collision detection and handling algorithms, and reduced subspace simulation methods to design and implement high-performance non-linear dynamics solvers.

        At present, my research is focused on multiscale methods for real-time convergent elastodynamics, robust geometry processing algorithms for cutting in virtual surgery simulations, and general neural physics primitives for solving PDEs on resource-constrained computational platforms.
        
        Please reach out to collaborate 😃

        <ins>*I am also actively looking for internship positions*</ins> 👨🏻‍💼
    design:
      spacing:
        padding: ['6rem', '10px', '6rem', '10px']
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Selected Publications
      filters:
        folders:
          - publication
    design:
      spacing:
        padding: ['6rem', '10px', '6rem', '10px']
      fill_image: false
      view: article-grid
      columns: 2
  - block: collection
    id: selected
    content:
      title: Publications
      filters:
        folders:
          - publication
    design:
      spacing:
        padding: ['0', '10px', '0', '10px']
      view: citation
  - block: collection
    id: projects
    content:
      title: Projects
      text: |- 
        Many researchers have a significantly higher bandwidth for designing algorithms than for implementing them. I try to leverage a strong foundation in software engineering to facilitate research velocity via contributions to open-source.

      filters:
        folders: 
          - project
    design:
      spacing:
        padding: ['6rem', '10px', '0', '10px']
      view: article-grid
      fill_image: false
      columns: 1
  - block: collection
    id: teaching
    content:
      title: Teaching
      filters:
        folders:
          - teaching
    design:
      view: card
      spacing:
        padding: ['6rem', '10px', 0, '10px']
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ""
      # Page type to display. E.g. post, talk, publication...
      page_type: docs
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - blog
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: ['6rem', '10px', 0, '10px']
---
