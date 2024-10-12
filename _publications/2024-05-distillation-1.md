---
title: "On Good Practices for Task-Specfici Distillation of Large Pretrained Visual Models"
collection: publications
category: manuscripts
permalink: /publication/2024-05-distillation
excerpt: '*Juliette Marrie, Michael Arbel, Julien Mairal, Diane Larlus*<br><br>This paper delineates good practices for leveraging current large pretrained visual models to train a small model on a specific task.'
date: 2024-05-02
venue: 'Transactions on Machine Learning Research (TMLR)'
paperurl: 'https://openreview.net/forum?id=oyISaaeHwD'
---

*Juliette Marrie, Michael Arbel, Julien Mairal, Diane Larlus*

Large pretrained visual models exhibit remarkable generalization across diverse recognition tasks. Yet, real-world applications often demand compact models tailored to specific problems. Variants of knowledge distillation have been devised for such a purpose, enabling task-specific compact models (the students) to learn from a generic large pretrained one (the teacher). In this paper, we show that the excellent robustness and versatility of recent pretrained models challenge common practices established in the literature, calling for a new set of optimal guidelines for task-specific distillation. To address the lack of samples in downstream tasks, we also show that a variant of Mixup based on stable diffusion complements standard data augmentation. This strategy eliminates the need for engineered text prompts and improves distillation of generic models into streamlined specialized networks.
