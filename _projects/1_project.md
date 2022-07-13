---
layout: page
title: Segmental Contrastive Predictive Coding for Unsupervised Word Segmentation
description: 
img: assets/img/SCPC.png
importance: 1
category: work
---

<object data="../assets/pdf/SCPC_fig.pdf" width="1000" height="1000" type='application/pdf'>
</object>


Automatic discovery of phone or word-like units is one of the core objectives in zero-resource speech processing. Recent attempts employ contrastive predictive coding (CPC), where the model learns representations by predicting the next frame given past context. However, CPC only looks at the audio signal's structure at the frame level. The speech structure exists beyond frame-level, i.e., at phone level or even higher. We propose a segmental contrastive predictive coding (SCPC) framework to learn from the signal structure at both the frame and phone levels.

SCPC is a hierarchical model with three stages trained in an end-to-end manner. In the first stage, the model predicts future feature frames and extracts frame-level representation from the raw waveform. In the second stage, a differentiable boundary detector finds variable-length segments. In the last stage, the model predicts future segments to learn segment representations. Experiments show that our model outperforms existing phone and word segmentation methods on TIMIT and Buckeye datasets.
