---
title: "DeepVenom: Persistent DNN Backdoors Exploiting Transient Weight Perturbations in Memories"
collection: publications
category: conferences
istop: istop
series: SP'24
authors: Cai, Kunbei and Chowdhuryy, Md Hafizul Islam and Zhang, Zhenkai and Yao, Fan
year: 2024
permalink: /publication/2/1/2024-deepvenom
excerpt: 'Backdoor attacks have raised significant concerns in machine learning (ML) systems. Mainstream ML backdoor attacks typically involve either poisoning the victim’s training samples or pre-training poisoned models for use by victim users. Meanwhile, recent advances in hardware-based threats reveal that ML model integrity at inference-time can be seriously tampered by inducing transient faults in model weights. However, the adversarial impacts of such hardware fault attacks at training time have ...'
date: 2/1/2024
venue: 'IEEE Symposium on Security and Privacy (SP)'
slidesurl: '../files/metaleak_slides.pdf'
paperurl: '../files/deepvenom.pdf'
citation: 'K. Cai, M. H. I. Chowdhuryy, Z. Zhang, and F. Yao, “Deepvenom: Persistent dnn backdoors exploiting transient weight perturbations,” in IEEE S&amp;P, 2024'
---
Backdoor attacks have raised significant concerns in machine learning (ML) systems. Mainstream ML backdoor attacks typically involve either poisoning the victim’s training samples or pre-training poisoned models for use by victim users. Meanwhile, recent advances in hardware-based threats reveal that ML model integrity at inference-time can be seriously tampered by inducing transient faults in model weights. However, the adversarial impacts of such hardware fault attacks at training time have not been well understood.In this paper, we present DeepVenom, the first end-to-end hardware-based DNN backdoor attack during victim model training. Particularly, DeepVenom can insert a targeted backdoor persistently at the victim model fine-tuning runtime through transient faults in model weight memory (via rowhammer). DeepVenom manifests in two main steps: i) an offline step that identifies weight perturbation transferable to the victim model using an ensemble-based local model bit search algorithm, and ii) an online stage that integrates advanced system-level techniques to efficiently massage weight tensors for precise rowhammer-based bit flips. DeepVenom further employs a novel iterative backdoor boosting mechanism that performs multiple rounds of weight perturbations to stabilize the backdoor. We implement an end-to-end DeepVenom attack in real systems with DDR3/DDR4 memories, and evaluate it using state-of-the-art Convolutional Neural Network and Vision Transformer models. The results show that DeepVenom can effectively generate backdoors in victim’s fine-tuned models with upto 99.8% attack success rate (97.8% on average) using as few as 11 total weight bit flips (maximum 49). The evaluation further demonstrates that DeepVenom is successful under varying victim fine-tuning hyperparameter settings, and is highly robust against catastrophic forgetting. Our work highlights the practicality of training-time backdoors through hardware-based weight perturbation, which represents a new dimension in adversarial machine learning.

[Download slides here](../files/metaleak_slides.pdf)

[Download paper here](../files/deepvenom.pdf)

Recommended citation: K. Cai, M. H. I. Chowdhuryy, Z. Zhang, and F. Yao, “Deepvenom: Persistent dnn backdoors exploiting transient weight perturbations,” in IEEE S&P, 2024