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
        <div class="space-y-5 mt-1">
          <div class="flex gap-x-6 items-baseline">
            <div class="shrink-0 w-24 text-xs font-semibold uppercase tracking-wider text-primary-600 dark:text-primary-400">Supervisors</div>
            <div>I am a PhD researcher at the <strong>Robert Koch Institute</strong> and <strong>Charité – Universitätsmedizin Berlin</strong>, supervised by <strong><a href="https://www.rki.de/DE/Institut/Organisation/Abteilungen/ZKI-PH/ZKI-PH3/zki-ph3-bildanalyse-node.html">Dr. Nils Körber</a></strong> (group leader, RKI, Image Analysis), <strong><a href="https://scholar.google.com/citations?user=A979AbYAAAAJ&hl=en">Prof. Grégoire Montavon</a></strong> (academic supervisor, BIFOLD/Charité, AI in Medicine), and <strong><a href="https://scholar.google.com/citations?user=5Dtr2nMAAAAJ&hl=de">Dr. Claudia Kohl</a></strong> (supervisor, RKI, Virological S3 Lab).</div>
          </div>
          <div class="flex gap-x-6 items-baseline">
            <div class="shrink-0 w-24 text-xs font-semibold uppercase tracking-wider text-primary-600 dark:text-primary-400">Methods</div>
            <div>On the methods side, I propose general-purpose frameworks for learning under difficult label conditions: <a href="publications/drainage">Drainage</a> (CVPR 2026 Highlight) is a unified framework for handling noisy labels, class ambiguity, and anomalous samples; <a href="publications/conveyance">Conveyance</a> is a structured loss function for classification over graph-like class hierarchies, designed to be domain-agnostic wherever class relationships carry meaningful structure, with particular utility in medical settings where label noise is itself structured.</div>
          </div>
          <div class="flex gap-x-6 items-baseline">
            <div class="shrink-0 w-24 text-xs font-semibold uppercase tracking-wider text-primary-600 dark:text-primary-400">Applied</div>
            <div>The application domain is viral diagnostics: detecting infected cell cultures at RKI, including pathogens that produce little or no visible cytopathic effect, where label noise, class structure, and distribution shift are practical realities rather than benchmarks.</div>
          </div>
          <div class="flex gap-x-6 items-baseline">
            <div class="shrink-0 w-24 text-xs font-semibold uppercase tracking-wider text-primary-600 dark:text-primary-400">Prior Work</div>
            <div>Earlier work includes an explainable RNA language model for small RNA biomarker annotation and lung cancer diagnostics (<a href="publications/transforna">TransfoRNA</a>); a GNN-based pharmaceutical cross-selling recommender deployed in production, addressing popularity bias in purchasing data (<a href="publications/pharmacy-gnn">PharmaSage</a>); and an extension of unsupervised monocular depth estimation via joint depth-optical-flow learning (<a href="publications/depth-prediction">Depth Prediction</a>), supervised by <strong><a href="https://scholar.google.com/citations?user=H_ICOW4AAAAJ&hl=de">Dr. Bernhard Nessler</a></strong> and <strong><a href="https://scholar.google.com/citations?user=tvUH3WMAAAAJ&hl=en">Prof. Sepp Hochreiter</a></strong> at JKU Linz.</div>
          </div>
        </div>

        Feel free to reach out to discuss collaborations or ideas [📬](mailto:tahay@rki.de)
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
