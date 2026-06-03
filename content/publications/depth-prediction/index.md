---
title: 'Unsupervised Depth Prediction from Monocular Images'

authors:
  - me

date: '2018-05-01T00:00:00Z'
publishDate: '2018-05-01T00:00:00Z'

publication_types: ['report']

publication:
  name: "Institute for Machine Learning, Johannes Kepler University Linz"
  short_name: "JKU Linz"

featured: true

abstract: >
  Supervised monocular depth estimation requires expensive ground-truth annotation.
  This work extends the DF-Net unsupervised framework — which jointly trains depth and
  optical flow subnetworks via photometric, smoothness, and cross-task consistency losses —
  with two novel loss terms. The **Mask Consistency Loss** enforces agreement between the
  valid-pixel masks produced independently by the depth and flow subnetworks,
  exploiting the fact that both masks should identify the same dynamic regions.
  Because mask generation is non-differentiable, consistency is enforced differentiably
  through the underlying flow representations. The **Mask Edge Aware Loss** penalises
  delta-flow in regions lacking image gradient, preventing the network from generating
  spurious depth boundaries unrelated to scene structure.

  Evaluated on the KITTI benchmark, the method achieves an Absolute Relative depth error
  of **0.146**, surpassing all contemporary unsupervised approaches including DF-Net
  (0.150), Godard et al. (0.154), and GeoNet (0.155). Optical flow estimation likewise
  improves on the K12 and K15 benchmarks. Qualitative analysis shows more defined edges,
  higher depth range, and fewer missed objects — with the main remaining failure mode
  being over-illuminated stationary surfaces shared across all methods.

  *Presented internally at the Institute for Machine Learning, JKU Linz, under the
  supervision of Dr. Bernhard Nesslar and Prof. Sepp Hochreiter.*

links:
  - name: "Slides"
    url: "Unsupervised_Depth_Prediction_from_Monocular_Images.pdf"
    icon: hero/presentation-chart-bar
---
