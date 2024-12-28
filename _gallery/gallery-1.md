---
layout: gallery
title: "LUDVIG: Learning-free Uplifting of 2D Visual features to Gaussian Splatting scenes"
media:
  - type: image
    src: /files/ludvig.png
    caption: "Illustration of the inverse and forward rendering between 2D visual features (produced by DINOv2) and a 3D Gaussian Splatting scene. In the inverse rendering (or uplifting) phase, features are created for each 3D Gaussian by aggregating coarse 2D features over all viewing directions. For forward rendering, the 3D features are projected on any given viewing direction as in regular Gaussian Splatting."
  - type: video
    src: /files/diffusion.mp4
    caption: "3D graph diffusion for foreground/background segmentation. The 3D mask spreads to neighboring Gaussians with similar DINOv2 features."
    format: mp4
  - type: video
    src: /files/figurines.mp4
    format: mp4
  - type: video
    src: /files/teatime.mp4
    format: mp4
    caption: "3D DINOv2 features (left), CLIP features (middle) and CLIP relevancy with text prompts (right)."
span_three_lines: True
description: "Recently, I worked on transferring representations from DINOv2, SAM, and CLIP into 3D Gaussian Splatting scenes. My study showed that a simple aggregation of 2D features is highly effective, achieving competitive results on segmentation and detection tasks while providing significant speed-ups over prior methods minimizing a reprojection loss. For 3D segmentation, we introduce a graph diffusion mechanism that enriches 3D features, such as coarse segmentation masks, by leveraging 3D geometry and pairwise similarities induced by DINOv2."
---

