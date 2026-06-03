---
title:  "Persona-Conditioned and Explainable Bikeability Assessment: A Multi-modal LLM Approach"
mathjax: true
layout: post
categories: 
 - aibigdata
---


<img align="left" width="317" height="353" src="https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/BikeabilityAssessment.png" style="vertical-align:middle;margin:15px 15px"/> Advancing human-centered infrastructure requires assessment approaches that consider users' subjective perceptions and preferences. Bikeability assessment is a representative case where user-centric evaluation must incorporate perceived safety and comfort across diverse cycling groups. Existing perception-based bikeability assessments face fundamental challenges for which Multi-modal large language models (MLLMs) offer a promising solution. However, the application of MLLMs in this domain faces another challenge: lack of supervision signal. That is, existing bikeability assessment approaches and datasets only provide scalar ratings, with no labels for factor attribution or reasoning traces, leaving MLLMs without the supervision signal needed to learn accurate rating prediction and robust chain-of-thought reasoning. In this paper, we propose a persona-conditioned framework that closes these supervision gaps and fine-tunes an MLLM end-to-end. The framework consists of: (i) counterfactual street-view augmentation for data scaling and per-feature attribution; (ii) an LLM-normalized factor vocabulary that unifies controlled and free-text survey responses; and (iii) persona-conditioned multi-granularity fine-tuning that jointly predicts ratings, identifies influencing factors, and generates explanations. 

*Key words: Bikeability; LLM, Generative AI, chain-of-thought, human-centered infrastructure*

* Related publication:

Dai, Y., Wang, Z., Wang, C., Zhou, K., Qian, Y., Xu, S., Yan, X. Persona-Conditioned and Explainable Bikeability Assessment: A Multi-modal LLM Approach. [Download Preprint](https://arxiv.org/html/2601.03534v1).



