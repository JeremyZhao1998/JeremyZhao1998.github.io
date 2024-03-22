---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

This section lists the selections of my publications.  
You can also find my articles on my <u><a href="https://scholar.google.com/citations?user=frRNkzkAAAAJ">Google Scholar profile</a></u>, and my academic activities on my <u><a href="https://orcid.org/0000-0001-9810-1122">ORCID</a></u>.  

{% include base_path %}

***

## Masked Retraining Teacher-student Framework for Domain Adaptive Object Detection  

**Zijing Zhao**, Sitong Wei, Qingchao Chen, Dehui Li, Yifan Yang, Yuxin Peng, Yang Liu†  

International Conference on Computer Vision (**ICCV**), 2023  

<div align="center">
  <img src="https://jeremyzhao1998.github.io/images/2023-mrt.png" alt="2023-mrt" width="500" />
</div>

<details>
  <summary>Abstract</summary>
  Domain adaptive Object Detection (DAOD) leverages a labeled domain (source) to learn an object detector generalizing to a novel domain without annotation (target). Recent advances use a teacher-student framework, i.e., a student model is supervised by the pseudo labels from a teacher model. Though great success, they suffer from the limited number of pseudo boxes with incorrect predictions caused by the domain shift, misleading the student model to get sub-optimal results. To mitigate this problem, we propose Masked Retraining Teacher-student framework (MRT) which leverages masked autoencoder and selective retraining mechanism on detection transformer. Specifically, we present a customized design of masked autoencoder branch, masking the multi-scale feature maps of target images and reconstructing features by the encoder of the student model and an auxiliary decoder. This helps the student model capture target domain characteristics and become a more data-efficient learner to gain knowledge from the limited number of pseudo boxes. Furthermore, we adopt selective retraining mechanism, periodically re-initializing certain parts of the student parameters with masked autoencoder refined weights to allow the model to jump out of the local optimum biased to the incorrect pseudo labels. Experimental results on three DAOD benchmarks demonstrate the effectiveness of our method.
</details>

***

## SAMP: A Model Inference Toolkit of Post-Training Quantization for Text Processing via Self-Adaptive Mixed-Precision
Rong Tian†, **Zijing Zhao**, Weijie Liu, Haoyan Liu, Weiquan Mao, Zhe Zhao, Kan Zhou  
Conference on Empirical Methods in Natural Language Processing: Industry Track (**EMNLP** Industry Track), 2023  
<div align="center">
  <img src="https://jeremyzhao1998.github.io/images/2023-samp.png" alt="2023-samp" width="200" />
</div>
