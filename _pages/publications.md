---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

This section lists the selections of my publications in time order.  
You can also find my articles on my <u><a href="https://scholar.google.com/citations?user=frRNkzkAAAAJ">Google Scholar profile</a></u>, and my academic activities on my <u><a href="https://orcid.org/0000-0001-9810-1122">ORCID</a></u>.  

\* denotes equal contribution, &dagger; denotes corresponding author.  

{% include base_path %}

***

***

## SIGMark: Scalable In-Generation Watermark with Blind Extraction for Video Diffusion

Xinjie Zhu\*, **Zijing Zhao**\*, Hui Jin, Qingxiao Guo, Yilong Ma, Yunhao Wang, Xiaobing Guo, Weifeng Zhang&dagger;  
Published as a conference paper at _International Conference on Learning Representations (**ICLR 2026**)_  
[[homepage](https://jeremyzhao1998.github.io/SIGMark-release/)] [[arxiv](https://arxiv.org/abs/2603.02882)] [[pdf](https://openreview.net/pdf?id=tKyAD2LhnI)] [[supp](https://openreview.net/attachment?id=tKyAD2LhnI&name=supplementary_material)] [[code](https://github.com/JeremyZhao1998/SIGMark-release)]  

<div align="center">  
  <img src="{{ base_path }}/images/2026-sigmark.png" alt="2026-sigmark" width="700" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  Artificial Intelligence Generated Content (AIGC), particularly video generation with diffusion models, has been advanced rapidly. Invisible watermarking is a key technology for protecting AI-generated videos and tracing harmful content, and thus plays a crucial role in AI safety. Beyond post-processing watermarks which inevitably degrade video quality, recent studies have proposed distortion-free in-generation watermarking for video diffusion models. However, existing in-generation approaches are non-blind: they require maintaining all the message-key pairs and performing template-based matching during extraction, which incurs prohibitive computational costs at scale. Moreover, when applied to modern video diffusion models with causal 3D Variational Autoencoders (VAEs), their robustness against temporal disturbance becomes extremely weak. To overcome these challenges, we propose SIGMark, a Scalable In-Generation watermarking framework with blind extraction for video diffusion. To achieve blind-extraction, we propose to generate watermarked initial noise using a Global set of Frame-wise PseudoRandom Coding keys (GF-PRC), reducing the cost of storing large-scale information while preserving noise distribution and diversity for distortion-free watermarking. To enhance robustness, we further design a Segment Group-Ordering module (SGO) tailored to causal 3D VAEs, ensuring robust watermark inversion during extraction under temporal disturbance. Comprehensive experiments on modern diffusion models show that SIGMark achieves very high bit-accuracy during extraction under both temporal and spatial disturbances with minimal overhead, demonstrating its scalability and robustness.  
</details>  

***

***

## Confidence-Aware Pseudo-Label Self-Correction for Weakly Supervised Visual Grounding

Yang Liu, Jiahua Zhang, Yue Wu, **Zijing Zhao**, Qingchao Chen, Yuxin Peng&dagger;  
Published in _IEEE Transactions on Pattern Analysis and Machine Intelligence (**TPAMI 2026**)_  
[[ieee](https://ieeexplore.ieee.org/abstract/document/11433810)]  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  Weakly supervised visual grounding aims to locate a region in an image based on an input query sentence, without access to the mapping between image regions and queries during training. Current methods treat spatial grounding as an object retrieval task, relying on cross-modal similarity scores for proposal selection. However, they fail to address model overfitting caused by unreliable cross-modal similarity scores. To overcome this, we first propose the Confidence-aware Pseudo-label Learning (CPL) framework. CPL first generates diverse pseudo queries for region proposals, and then establishes reliable associations for model training based on the uni-modal similarity score. Secondly, we propose a cross-modal verification module based on the pretrained vision-language model to verify associations. However, the verification module is isolated from the grounding model, so it can only assess associations in a static manner, but not correct the suspicious ones. Finally, we introduce CPL++ to make two-fold improvements. For one thing, we upgrade the verification process based on the model's grounding loss value to identify suspicious associations dynamically and selectively leverage them in the training. For another, we propose a self-supervised association correction module to rectify suspicious associations, thereby mitigating the risk of error propagation. Experimental results on five datasets demonstrate the superiority of our approach.  
</details>  

***

***

## Investigating Domain Gaps for Indoor 3D Object Detection

**Zijing Zhao**, Zhu Xu, Qingchao Chen, Yuxin Peng, Yang Liu&dagger;  
Published on _ACM International Conference on Multimedia (**ACM MM 2025**)_ (CCF-A)  
[[arxiv](https://www.arxiv.org/abs/2508.17439)] [[code](https://github.com/JeremyZhao1998/DAVoteNet-release)] [[homepage](https://jeremyzhao1998.github.io/DAVoteNet-release/)]  

<div align="center">  
  <img src="{{ base_path }}/images/2025-davotenet.png" alt="2025-davotenet" width="700" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  As a fundamental task for indoor scene understanding, 3D object detection has been extensively studied, and the accuracy on indoor point cloud data has been substantially improved. However, existing researches have been conducted on limited datasets, where the training and testing sets share the same distribution. In this paper, we consider the task of adapting indoor 3D object detectors from one dataset to another, presenting a comprehensive benchmark with ScanNet, SUN RGB-D and 3D Front datasets, as well as our newly proposed large-scale datasets ProcTHOR-OD and ProcFront generated by a 3D simulator. Since indoor point cloud datasets are collected and constructed in different ways, the object detectors are likely to overfit to specific factors within each dataset, such as point cloud quality, bounding box layout and instance features. We conduct experiments across datasets on different adaptation scenarios including synthetic-to-real adaptation, point cloud quality adaptation, layout adaptation and instance feature adaptation, analyzing the impact of different domain gaps on 3D object detectors. We also introduce several approaches to improve adaptation performances, providing baselines for domain adaptive indoor 3D object detection, hoping that future works may propose detectors with stronger generalization ability across domains.  
</details>  

***

***

## Zero Shot Domain Adaptive Semantic Segmentation by Synthetic Data Generation and Progressive Adaptation

Jun Luo, **Zijing Zhao**, Yang Liu&dagger;  
Published on _IEEE/RSJ International Conference on Intelligent Robots and Systems (**IROS 2025**)_ (**Oral**)  
[[arxiv](https://arxiv.org/abs/2508.03300v1)] [[code](https://github.com/ROUJINN/SDGPA)]  

<div align="center">  
  <img src="{{ base_path }}/images/2025-sdgpa.png" alt="2025-sdgpa" width="700" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  Deep learning-based semantic segmentation models achieve impressive results yet remain limited in handling distribution shifts between training and test data. In this paper, we present SDGPA (Synthetic Data Generation and Progressive Adaptation), a novel method that tackles zero-shot domain adaptive semantic segmentation, in which no target images are available, but only a text description of the target domain's style is provided. To compensate for the lack of target domain training data, we utilize a pretrained off-the-shelf text-to-image diffusion model, which generates training images by transferring source domain images to target style. Directly editing source domain images introduces noise that harms segmentation because the layout of source images cannot be precisely maintained. To address inaccurate layouts in synthetic data, we propose a method that crops the source image, edits small patches individually, and then merges them back together, which helps improve spatial precision. Recognizing the large domain gap, SDGPA constructs an augmented intermediate domain, leveraging easier adaptation subtasks to enable more stable model adaptation to the target domain. Additionally, to mitigate the impact of noise in synthetic data, we design a progressive adaptation strategy, ensuring robust learning throughout the training process. Extensive experiments demonstrate that our method achieves state-of-the-art performance in zero-shot semantic segmentation.  
</details>  

***

***

## AR-VRM: Imitating Human Motions for Visual Robot Manipulation with Analogical Reasoning

Dejie Yang, **Zijing Zhao**, Yang Liu&dagger;  
Published on _The IEEE/CVF International Conference on Computer Vision (**ICCV 2025**)_ (CCF-A)  
[[arxiv](https://arxiv.org/abs/2508.07626)] [[code](https://github.com/idejie/AR)] [[homepage](https://idejie.com/AR/)]  

<div align="center">  
  <img src="{{ base_path }}/images/2025-ar-vrm.png" alt="2025-ar-vrm" width="700" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  Visual Robot Manipulation (VRM) aims to enable a robot to follow natural language instructions based on robot states and visual observations, and therefore requires costly multi-modal data. To compensate for the deficiency of robot data, existing approaches have employed vision-language pretraining with large-scale data. However, they either utilize web data that differs from robotic tasks, or train the model in an implicit way (e.g., predicting future frames at the pixel level), thus showing limited generalization ability under insufficient robot data. In this paper, we propose to learn from large-scale human action video datasets in an explicit way (i.e., imitating human actions from hand keypoints), introducing Visual Robot Manipulation with Analogical Reasoning (AR-VRM). To acquire action knowledge explicitly from human action videos, we propose a keypoint Vision-Language Model (VLM) pretraining scheme, enabling the VLM to learn human action knowledge and directly predict human hand keypoints. During fine-tuning on robot data, to facilitate the robotic arm in imitating the action patterns of human motions, we first retrieve human action videos that perform similar manipulation tasks and have similar historical observations, and then learn the Analogical Reasoning (AR) map between human hand keypoints and robot components. Taking advantage of focusing on action keypoints instead of irrelevant visual cues, our method achieves leading performance on the CALVIN benchmark and real-world experiments. In few-shot scenarios, our AR-VRM outperforms previous methods by large margins, underscoring the effectiveness of explicitly imitating human actions under data scarcity.  
</details>  

***

***

## PlanLLM: Video Procedure Planning with Refinable Large Language Models

Dejie Yang, **Zijing Zhao**, Yang Liu&dagger;  
Published on _The AAAI Conference on Artificial Intelligence (**AAAI 2025**)_ (CCF-A)  
[[pdf](https://ojs.aaai.org/index.php/AAAI/article/download/32992/35147)] [[code](https://github.com/idejie/PlanLLM)] [[project page](https://idejie.com/PlanLLM_pages/)]  

<div align="center">  
  <img src="{{ base_path }}/images/2025-planllm.png" alt="2025-planllm" width="700" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  Video procedure planning, ie, planning a sequence of action steps given the video frames of start and goal states, is an essential ability for embodied AI. Recent works utilize Large Language Models (LLMs) to generate enriched action step description texts to guide action step decoding. Although LLMs are introduced these methods decode the action steps into a closed-set of one-hot vectors, limiting the model's capability of generalizing to new steps or tasks. Additionally, fixed action step descriptions based on world-level commonsense may contain noise in specific instances of visual states. In this paper, we propose PlanLLM, a cross-modal joint learning framework with LLMs for video procedure planning. We propose an LLM-Enhanced Planning module which fully uses the generalization ability of LLMs to produce free-form planning output and to enhance action step decoding. We also propose Mutual Information Maximization module to connect world-level commonsense of step descriptions and sample-specific information of visual states, enabling LLMs to employ the reasoning ability to generate step sequences. With the assistance of LLMs, our method can both closed-set and open vocabulary procedure planning tasks. Our PlanLLM achieves superior performance on three benchmarks, demonstrating the effectiveness of our designs.  
</details>  

***

***

## Masked Retraining Teacher-student Framework for Domain Adaptive Object Detection

**Zijing Zhao**, Sitong Wei, Qingchao Chen, Dehui Li, Yifan Yang, Yuxin Peng, Yang Liu&dagger;  
Published on _International Conference on Computer Vision (**ICCV 2023**)_ (CCF-A)  
[[pdf](https://openaccess.thecvf.com/content/ICCV2023/papers/Zhao_Masked_Retraining_Teacher-Student_Framework_for_Domain_Adaptive_Object_Detection_ICCV_2023_paper.pdf)] [[supp](https://openaccess.thecvf.com/content/ICCV2023/supplemental/Zhao_Masked_Retraining_Teacher-Student_ICCV_2023_supplemental.pdf)] [[code](https://github.com/JeremyZhao1998/MRT-release)] [[homepage](https://jeremyzhao1998.github.io/MRT-release/)]  

<div align="center">  
  <img src="{{ base_path }}/images/2023-mrt.png" alt="2023-mrt" width="700" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  Domain adaptive Object Detection (DAOD) leverages a labeled domain (source) to learn an object detector generalizing to a novel domain without annotation (target). Recent advances use a teacher-student framework, i.e., a student model is supervised by the pseudo labels from a teacher model. Though great success, they suffer from the limited number of pseudo boxes with incorrect predictions caused by the domain shift, misleading the student model to get sub-optimal results. To mitigate this problem, we propose Masked Retraining Teacher-student framework (MRT) which leverages masked autoencoder and selective retraining mechanism on detection transformer. Specifically, we present a customized design of masked autoencoder branch, masking the multi-scale feature maps of target images and reconstructing features by the encoder of the student model and an auxiliary decoder. This helps the student model capture target domain characteristics and become a more data-efficient learner to gain knowledge from the limited number of pseudo boxes. Furthermore, we adopt selective retraining mechanism, periodically re-initializing certain parts of the student parameters with masked autoencoder refined weights to allow the model to jump out of the local optimum biased to the incorrect pseudo labels. Experimental results on three DAOD benchmarks demonstrate the effectiveness of our method.  
</details>  

***

***

## SAMP: A Model Inference Toolkit of Post-Training Quantization for Text Processing via Self-Adaptive Mixed-Precision

Rong Tian&dagger;, **Zijing Zhao**, Weijie Liu, Haoyan Liu, Weiquan Mao, Zhe Zhao, Kan Zhou  
Published on _Conference on Empirical Methods in Natural Language Processing: Industry Track (**EMNLP 2023**)_ (CCF-B)  
[[pdf](https://aclanthology.org/2023.emnlp-industry.13.pdf)]  

<div align="center">  
  <img src="{{ base_path }}/images/2023-samp.png" alt="2023-samp" width="350" />  
</div>  

<details>  
  <summary>Abstract (Click to unfold): </summary>  
  The latest industrial inference engines, such as FasterTransformer1 and TurboTransformers, have verified that halfprecision floating point (FP16) and 8-bit integer (INT8) quantization can greatly improve model inference speed. However, the existing INT8 quantization methods are too complicated, and improper usage will lead to model performance damage greatly. In this paper, we develop a toolkit for users to easily quantize their models for inference, in which Self-Adaptive MixedPrecision (SAMP) is proposed to automatically control quantization rate by a mixed-precision architecture to balance model accuracy and efficiency. Experimental results show that our SAMP toolkit has a higher speedup than PyTorch and FasterTransformer while ensuring the required accuracy. In addition, SAMP is based on a modular design, decoupling the tokenizer, embedding, encoder and target layers, which allows users to handle various downstream tasks and can be seamlessly integrated into PyTorch.  
</details>  
