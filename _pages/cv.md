---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. in Computer Science, Northeastern University, GPA: 4.0 / 4.0, Sep. 2023 - Apr. 2026 (expected)
* B.S. in Mathematics, University of Colorado at Denver, GPA: 3.5 / 4.0, Sep. 2019 - May 2024

Research Interests
======
Diffusion Models, Vision-Language Models, Model Generalization, Parameter-Efficient Fine-Tuning

Research Experience
======
### Research Assistant — MMLAB @ SIAT, Chinese Academy of Sciences, Shenzhen  
**Nov. 2024 – Aug. 2025**

**Generalizable VLM Fine-tuning Methods**
* Developed **GLAD**, a generalizable fine-tuning framework for vision-language models in few-shot settings.
* Investigated limitations of CLIP prompt tuning and identified causes of overfitting.
* Proposed a **LoRA-based** cross-modal fine-tuning strategy updating only a small portion of parameters.
* Designed **AlignNet**, a lightweight alignment module to enhance text embeddings using image-aware cues.
* Introduced **SAM-inspired gradient regularization** to improve robustness and guide optimization toward flatter minima.
* Conducted evaluations on **15 datasets**, covering base-to-novel generalization and domain transfer.
* Demonstrated that GLAD outperforms CoOp, CoCoOp, MaPLe, and PromptSRC.
* Led the full project: conceptualization, method design, implementation, large-scale benchmarking, and writing.

**Personalized Image Editing via Diffusion Models**
* Developed **TARA**, a framework enabling training-free multi-concept image generation with diffusion models.
* Identified **token interference** and **spatial misalignment** as key issues in LoRA-based personalization.
* Designed **Token Focus Masking (TFM)** to constrain each LoRA update to its associated rare token.
* Proposed **Token Alignment Loss (TAL)** to enforce alignment between rare-token attention and class-token regions.
* Implemented TARA on **Stable Diffusion v1.5 & SDXL**, enabling multi-concept composition during inference.
* Conducted experiments on DreamBooth datasets using CLIP-T, CLIP-I, DINO metrics.
* Demonstrated superior identity preservation over DB-LoRA, Mix-of-Show, and other baselines.
* Led the full project from algorithm design, implementation, ablation studies, to manuscript writing.

Course Projects
======

### Data-Efficient Subset Selection for Image Classification — Northeastern University, 2024
* Built a data-centric selection system using **submodular optimization** to choose diverse and informative samples.
* Analyzed limits of dataset distillation and random subset selection.
* Used **ResNet-18** to extract features and guide iterative sample selection.
* Evaluated subsets (10%–50%) on ResNet-18/50/101 and ViT.
* Achieved **89.16% accuracy** at 50% subset size (vs. 82.17% for random), approaching full-data accuracy of 92.14%.

Work Experience
======

### MIIVII Technology, Beijing — Research Intern  
**May 2024 – Sept. 2024**
* Annotated **3D point cloud motion data** aligned with RGB video.
* Investigated **NeRF-based mesh extraction** and evaluated performance on internal datasets.

Publications
======
<ul>
<li>Y. Peng, P. Wang, J. Liu, S. Chen. <strong>"GLAD: Generalizable Tuning for Vision-Language Models."</strong> ICCV Workshops, 2025. [PDF]</li>
<li>Y. Peng, L. Zheng, Y. Yang, Y. Huang, M. Yan, J. Liu, S. Chen. <strong>"TARA: Token-Aware LoRA for Composable Personalization in Diffusion Models."</strong> 2025. (Submitted to AAAI) [PDF]</li>
</ul>

Honors & Awards
======
* First Place — “Yuan Geng Cup” Shenzhen Badminton Tournament, 2025  
* First Place — USA National Collegiate Team Badminton Championships, 2024  
* Third Place — “Li-Ning Cup” Beijing University Division (Men’s Singles), 2018  

Technical Skills
======
* **Programming:** Python, Java, C, C++, R, Swift  
* **Deep Learning Frameworks:** PyTorch
  

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  

