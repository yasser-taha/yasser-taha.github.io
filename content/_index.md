---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I am a PhD researcher at the **Robert Koch Institute** and **Charité – Universitätsmedizin Berlin**, supervised by **Prof. Grégoire Montavon** (academic supervisor, Charité — AI in Medicine), **Dr. Nils Körber** (group leader, RKI — Image Analysis), and **Dr. Claudia Kohl** (supervisor, RKI — Virological S3 Lab).

        My work is split between **foundational ML research** and its **application to real-world virology**. On the methods side, I develop general-purpose frameworks for learning under difficult label conditions: [Drainage](publications/drainage) (CVPR 2026 Highlight) is a unified framework for handling noisy labels, class ambiguity, and anomalous samples; [Conveyance](publications/conveyance) is a structured loss function for classification over graph-like class hierarchies, covering ordinal regression, hierarchical classification, and multiple instance learning.

        On the applied side, I use these and related ideas to build tools for detecting virus-infected cell cultures at RKI — including infections that produce little or no visible cytopathic effect — where label noise, class structure, and distribution shift are practical realities rather than benchmarks.

        Earlier work spans small RNA biomarker discovery for lung cancer diagnostics (TransfoRNA), pharmaceutical recommender systems via graph neural networks, and unsupervised monocular depth estimation — supervised by **Prof. Sepp Hochreiter** at JKU Linz.

        Feel free to reach out to discuss collaborations or ideas 📬
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Projects
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 10
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]

---
