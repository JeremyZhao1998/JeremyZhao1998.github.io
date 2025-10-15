---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

This section lists the selections of my publications in time order.  
You can also find my articles on my <u><a href="https://scholar.google.com/citations?user=frRNkzkAAAAJ">Google Scholar profile</a></u>, and my academic activities on my <u><a href="https://orcid.org/0000-0001-9810-1122">ORCID</a></u>.  

{% include base_path %}

***

***  

## PlanLLM: Video Procedure Planning with Refinable Large Language Models  

Dejie Yang, **Zijing Zhao** and Yang Liu†  
Published on _The AAAI Conference on Artificial Intelligence (**AAAI 2025**)_ (CCF-A)  
[[pdf](https://ojs.aaai.org/index.php/AAAI/article/download/32992/35147)] [[code](https://github.com/idejie/PlanLLM)] [[project page](https://idejie.com/PlanLLM_pages/)]   

<div align="center">  
  <img src="https://jeremyzhao1998.github.io/images/2025-planllm.png" alt="2023-mrt" width="700" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  Video procedure planning, ie, planning a sequence of action steps given the video frames of start and goal states, is an essential ability for embodied AI. Recent works utilize Large Language Models (LLMs) to generate enriched action step description texts to guide action step decoding. Although LLMs are introduced these methods decode the action steps into a closed-set of one-hot vectors, limiting the model's capability of generalizing to new steps or tasks. Additionally, fixed action step descriptions based on world-level commonsense may contain noise in specific instances of visual states. In this paper, we propose PlanLLM, a cross-modal joint learning framework with LLMs for video procedure planning. We propose an LLM-Enhanced Planning module which fully uses the generalization ability of LLMs to produce free-form planning output and to enhance action step decoding. We also propose Mutual Information Maximization module to connect world-level commonsense of step descriptions and sample-specific information of visual states, enabling LLMs to employ the reasoning ability to generate step sequences. With the assistance of LLMs, our method can both closed-set and open vocabulary procedure planning tasks. Our PlanLLM achieves superior performance on three benchmarks, demonstrating the effectiveness of our designs.  
</details>  

***

***  

## Masked Retraining Teacher-student Framework for Domain Adaptive Object Detection  

**Zijing Zhao**, Sitong Wei, Qingchao Chen, Dehui Li, Yifan Yang, Yuxin Peng and Yang Liu†  
Published on _International Conference on Computer Vision (**ICCV 2023**)_ (CCF-A)  
[[pdf](https://openaccess.thecvf.com/content/ICCV2023/papers/Zhao_Masked_Retraining_Teacher-Student_Framework_for_Domain_Adaptive_Object_Detection_ICCV_2023_paper.pdf)] [[supp](https://openaccess.thecvf.com/content/ICCV2023/supplemental/Zhao_Masked_Retraining_Teacher-Student_ICCV_2023_supplemental.pdf)] [[code](https://github.com/JeremyZhao1998/MRT-release)] [[homepage](https://jeremyzhao1998.github.io/MRT-release/)]  

<div align="center">  
  <img src="https://jeremyzhao1998.github.io/images/2023-mrt.png" alt="2023-mrt" width="700" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  Domain adaptive Object Detection (DAOD) leverages a labeled domain (source) to learn an object detector generalizing to a novel domain without annotation (target). Recent advances use a teacher-student framework, i.e., a student model is supervised by the pseudo labels from a teacher model. Though great success, they suffer from the limited number of pseudo boxes with incorrect predictions caused by the domain shift, misleading the student model to get sub-optimal results. To mitigate this problem, we propose Masked Retraining Teacher-student framework (MRT) which leverages masked autoencoder and selective retraining mechanism on detection transformer. Specifically, we present a customized design of masked autoencoder branch, masking the multi-scale feature maps of target images and reconstructing features by the encoder of the student model and an auxiliary decoder. This helps the student model capture target domain characteristics and become a more data-efficient learner to gain knowledge from the limited number of pseudo boxes. Furthermore, we adopt selective retraining mechanism, periodically re-initializing certain parts of the student parameters with masked autoencoder refined weights to allow the model to jump out of the local optimum biased to the incorrect pseudo labels. Experimental results on three DAOD benchmarks demonstrate the effectiveness of our method.  
</details>  

***  

***  

## SAMP: A Model Inference Toolkit of Post-Training Quantization for Text Processing via Self-Adaptive Mixed-Precision  

Rong Tian†, **Zijing Zhao**, Weijie Liu, Haoyan Liu, Weiquan Mao, Zhe Zhao and Kan Zhou  
Published on _Conference on Empirical Methods in Natural Language Processing: Industry Track (**EMNLP 2023**)_ (CCF-B)  
[[pdf](https://aclanthology.org/2023.emnlp-industry.13.pdf)]  

<div align="center">  
  <img src="https://jeremyzhao1998.github.io/images/2023-samp.png" alt="2023-samp" width="350" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  The latest industrial inference engines, such as FasterTransformer1 and TurboTransformers, have verified that halfprecision floating point (FP16) and 8-bit integer (INT8) quantization can greatly improve model inference speed. However, the existing INT8 quantization methods are too complicated, and improper usage will lead to model performance damage greatly. In this paper, we develop a toolkit for users to easily quantize their models for inference, in which Self-Adaptive MixedPrecision (SAMP) is proposed to automatically control quantization rate by a mixed-precision architecture to balance model accuracy and efficiency. Experimental results show that our SAMP toolkit has a higher speedup than PyTorch and FasterTransformer while ensuring the required accuracy. In addition, SAMP is based on a modular design, decoupling the tokenizer, embedding, encoder and target layers, which allows users to handle various downstream tasks and can be seamlessly integrated into PyTorch.  
</details>  
