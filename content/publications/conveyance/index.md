---
title: 'Conveyance: A Versatile Framework for Learning in Structured Class Spaces'

authors:
  - me
  - "Grégoire Montavon"
  - "Nils Körber"
author_notes:
  - ""
  - "Equal supervision"
  - "Equal supervision"

date: '2026-05-27T00:00:00Z'
publishDate: '2026-05-27T00:00:00Z'

publication_types: ['article']

peer_reviewed: false
open_access: true
license: CC-BY-4.0

abstract: >
  While machine learning (ML) architectures have evolved rapidly to account for
  complex data, loss functions like cross-entropy remain mostly structure-agnostic
  in many real-world applications. However, the "class-symmetric" nature of these
  standard losses fundamentally limits the ability of ML models to exploit
  structural relationships between classes, particularly when facing structured noise.
  We propose Conveyance, a new classification approach and associated loss function
  tailored to structured class spaces. It allows users to encode graph-like
  relations between classes without having to define complex joint distributions or
  manually tune utility matrices. Technically, our loss function operates by maximizing
  two separate margins over distinct class partitions, while preserving formal
  properties such as monotonicity and partial convexity. We demonstrate the
  versatility and effectiveness of our method by applying it to hierarchical
  classification, ordinal regression, and multiple instance learning. Across these
  tasks, Conveyance either matches or exceeds the performance of specialized baselines,
  thereby offering a unified solution for structured class spaces.

summary: >
  Conveyance is a new loss function and classification framework for structured
  class spaces that encodes graph-like class relations without manual tuning,
  achieving state-of-the-art results across hierarchical classification, ordinal
  regression, and multiple instance learning.

tags:
  - Structured Class Spaces
  - Annotation Bias
  - Structured Noise

featured: true

hugoblox:
  ids:
    doi: 10.48550/arXiv.2605.28420

links:
  - type: pdf
    url: "https://arxiv.org/pdf/2605.28420"
  - type: code
    url: "https://github.com/ZKI-PH-ImageAnalysis/Conveyance"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2605.28420"
---
> *I am currently working on a blog post with more details about this project — check back soon.*