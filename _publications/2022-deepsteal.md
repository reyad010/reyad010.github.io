---
title: "DeepSteal: Advanced Model Extractions Leveraging Efficient Weight Stealing in Memories"
collection: publications
category: conferences
istop: istop
series: SP'22
authors: Chowdhuryy, Md Hafizul Islam and Rakin, Adnan Siraj and Yao, Fan and Fan, Deliang
year: 2022
permalink: /publication/10/1/2022-deepsteal
excerpt: 'Recent advancements in Deep Neural Networks (DNNs) have enabled widespread deployment in multiple security-sensitive domains. The need for resource-intensive training and the use of valuable domain-specific training data have made these models the top intellectual property (IP) for model owners. One of the major threats to DNN privacy is model extraction attacks where adversaries attempt to steal sensitive information in DNN models. In this work, we propose an advanced model extraction ...'
date: 10/1/2022
venue: 'IEEE Symposium on Security and Privacy (SP)'
slidesurl: '../files/deepsteal_slides.pdf'
paperurl: '../files/deepsteal.pdf'
citation: 'M. H. I. Chowdhuryy, A. S. Rakin, F. Yao, and D. Fan, “Deepsteal: Advanced model extractions leveraging efficient weight stealing in memories,” 2022.'
---
Recent advancements in Deep Neural Networks (DNNs) have enabled widespread deployment in multiple security-sensitive domains. The need for resource-intensive training and the use of valuable domain-specific training data have made these models the top intellectual property (IP) for model owners. One of the major threats to DNN privacy is model extraction attacks where adversaries attempt to steal sensitive information in DNN models. In this work, we propose an advanced model extraction framework DeepSteal that steals DNN weights remotely for the first time with the aid of a memory side-channel attack. Our proposed DeepSteal comprises two key stages. Firstly, we develop a new weight bit information extraction method, called HammerLeak, through adopting the rowhammer-based fault technique as the information leakage vector. HammerLeak leverages several novel system-level techniques tailored for DNN applications to enable fast and efficient weight stealing. Secondly, we propose a novel substitute model training algorithm with Mean Clustering weight penalty, which leverages the partial leaked bit information effectively and generates a substitute prototype of the target victim model. We evaluate the proposed model extraction framework on three popular image datasets (e.g., CIFAR-10/100/GTSRB) and four DNN architectures (e.g., ResNet-18/34/Wide-ResNetNGG-11). The extracted substitute model has successfully achieved more than 90% test accuracy on deep residual networks for the CIFAR-10 dataset. Moreover, our extracted substitute model could also generate effective adversarial input samples to fool the victim model. Notably, it achieves similar performance (i.e., ~1-2% test accuracy under attack) as white-box adversarial input attack (e.g., PGD/Trades).

[Download slides here](../files/deepsteal_slides.pdf)

[Download paper here](../files/deepsteal.pdf)

Recommended citation: M. H. I. Chowdhuryy, A. S. Rakin, F. Yao, and D. Fan, “Deepsteal: Advanced model extractions leveraging efficient weight stealing in memories,” 2022.