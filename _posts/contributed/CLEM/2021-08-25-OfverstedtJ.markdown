---
title: "Fast Computation of Mutual Information with Application to Global Multimodal Image Alignment of Micrographs"
layout: post
date: 2021-08-25 14:00
image: 
headerImage: false
tag:
- contributed
- CLEM
category: projects
author:
#description: Markdown summary with different options
---

_**Johan Öfverstedt**, Joakim Lindblad, Nataša Sladoje._

MIDA Group, Department of Information Technology, Uppsala University, Uppsala, Sweden

## Abstract

Multimodal image alignment is the process of finding spatial correspondences between images formed by different imaging techniques, to facilitate heterogeneous data fusion and correlative analysis. Image alignment methods based on maximization of mutual information (MI) are well established and a part of most general-purpose multimodal image alignment packages. MI maximization is typically used in local optimization frameworks where an initial guess for the transformation parameters is required, and where the local region around this guess is explored, guided by the derivatives of MI. Local optimization often implies substantial robustness and usability challenges: (i) a good initial guess can be hard to find, (ii) the optimizer may fail to converge to the sought solution, and (iii) there tend to be many hyper-parameters to tune. These three challenges are likely to be present when applying MI to multimodal microscopy scenarios, due to sparseness of key structures, indistinct local features, and large displacements.

We recently proposed a novel algorithm for computing MI between two images for all discrete displacements. This algorithm, based on cross-correlation computed in the frequency domain, is substantially more efficient than existing algorithms – it is several orders of magnitude faster. Applying the algorithm for a suitable set of rotation angles, we obtain a global optimization method for rigid multimodal image alignment that successfully addresses the three previously listed challenges of local maximization of MI.

To evaluate the efficacy of the proposed method, we selected public benchmark datasets comprising aligned multimodal cytological image pairs (fluorescence and quantitative phase imaging (QPI)), and aligned multimodal histological image pairs (brightfield (BF) and second-harmonic generation (SHG) imaging), where each image was subjected to synthetic rigid transformations. We observed excellent performance, in terms of the rate of successful recovery of the known transformation, on both datasets, outperforming a number of existing methods with a wide margin, including local maximization of MI as well as recent deep learning-based approaches.

We implemented the method in PyTorch to enable the use of GPU acceleration to speed up the runtime and facilitate practical applicability. The implementation and reference to our full study is available at github.com/MIDA-group/globalign.