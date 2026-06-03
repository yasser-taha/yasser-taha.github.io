---
title: 'Drainage: A Unifying Framework for Addressing Class Uncertainty'

authors:
  - me
  - "Grégoire Montavon"
  - "Nils Körber"
author_notes:
  - ""
  - "Equal supervision"
  - "Equal supervision"

date: '2025-12-02T00:00:00Z'
publishDate: '2025-12-02T00:00:00Z'

publication_types: ['paper-conference']

publication:
  name: "IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)"
  short_name: "CVPR 2026"

peer_reviewed: true
open_access: true
license: arXiv

awards:
  - name: "Highlight Paper"
    level: selected
    note: "Top ~3.5% of submissions at CVPR 2026"

abstract: >
  Modern deep learning faces significant challenges with noisy labels, class
  ambiguity, as well as the need to robustly reject out-of-distribution or corrupted
  samples. In this work, we propose a unified framework based on the concept of a
  "drainage node" which we add at the output of the network. The node serves to
  reallocate probability mass toward uncertainty, while preserving desirable
  properties such as end-to-end training and differentiability. This mechanism provides a
  natural escape route for highly ambiguous, anomalous, or noisy samples,
  particularly relevant for instance-dependent and asymmetric label noise. In systematic
  experiments involving the addition of varying proportions of instance-dependent
  noise or asymmetric noise to CIFAR-10/100 labels, our drainage formulation
  achieves an accuracy increase of up to 9% over existing approaches in the high-noise
  regime. Our results on real-world datasets, such as mini-WebVision, mini-ImageNet
  and Clothing-1M, match or surpass existing state-of-the-art methods. Qualitative
  analysis reveals a denoising effect, where the drainage neuron consistently absorbs
  corrupt, mislabeled, or outlier data, leading to more stable decision boundaries.
  Furthermore, our drainage formulation enables applications well beyond
  classification, with immediate benefits for web-scale, semi-supervised dataset
  cleaning, and open-set applications.

summary: >
  We propose Drainage, a unified framework that adds a "drainage node" to the
  network output to handle noisy labels, class ambiguity, and out-of-distribution
  samples — achieving up to 9% accuracy gains over existing approaches on
  CIFAR-10/100 with instance-dependent noise. Highlighted at CVPR 2026.

tags:
  - Deep Learning
  - Noisy Labels
  - Out-of-Distribution Detection
  - Classification
  - Computer Vision

featured: true

hugoblox:
  ids:
    doi: 10.48550/arXiv.2512.03182

links:
  - type: pdf
    name: "arXiv PDF"
    url: "https://arxiv.org/pdf/2512.03182"
  - type: code
    url: "https://github.com/ZKI-PH-ImageAnalysis/Drainage"
  - type: video
    url: "https://youtu.be/U8jF3Og9gwc?si=P_QGwmE_UDG0tVk1"
  - name: "Poster"
    url: "CVPR2026_Poster.pptx"
  - name: "CVPR Virtual"
    url: "https://cvpr.thecvf.com/virtual/2026/poster/39457"
    icon: hero/computer-desktop
  - name: "arXiv"
    url: "https://arxiv.org/abs/2512.03182"
---
> *I am currently working on a blog post with more details about this project — check back soon.*