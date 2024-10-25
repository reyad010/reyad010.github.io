---
title: "PowSpectre: Powering Up Speculation Attacks with TSX-based Replay"
collection: publications
category: conferences
istop: isnottop
series: ASIACCS '24
authors: Chowdhuryy, Md Hafizul Islam and Zhang, Zhenkai and Yao, Fan
year: 2024
permalink: /publication/1/1/2024-powspectre
excerpt: 'Trusted execution environment (TEE) offers data protection against malicious system software. However, the TEE (e.g., Intel SGX) threat model exacerbates information leakage as attackers can enhance and denoise the observations from hardware-based side channels through controlled victim execution (i.e., replay). The replay mechanism is especially critical for side channels from physical traces (e.g., power consumption) that not only vary instantaneously but also necessitate successive ...'
date: 1/1/2024
venue: 'ACM Asia Conference on Computer and Communications Security (ASIACCS)'
slidesurl: '../files/powspectre_slides.pdf'
paperurl: '../files/powspectre.pdf'
citation: 'M. H. I. Chowdhuryy, Z. Zhang, and F. Yao, “Powspectre: Powering up speculation attacks with tsx-based replay,” in ACM ASIACCS, 2024.'
---
Trusted execution environment (TEE) offers data protection against malicious system software. However, the TEE (e.g., Intel SGX) threat model exacerbates information leakage as attackers can enhance and denoise the observations from hardware-based side channels through controlled victim execution (i.e., replay). The replay mechanism is especially critical for side channels from physical traces (e.g., power consumption) that not only vary instantaneously but also necessitate successive modulation for observability. In this paper, we identify and characterize the key limitations of existing replay techniques for speculation attacks. Our study unveils that architectural support for transactional memory (i.e., Intel TSX) can be leveraged as a highly efficient replay primitive for transient execution. Based on this observation, we design TMPlayer, an efficient and high-resolution TSX-based replay framework for enclave victims. Built on top of TMPlayer, we present PowSpectre- a novel replay-based transient execution attack using software-based power side channels (via RAPL) that can exfiltrate secretive enclave data accurately in the speculative domain. We evaluate PowSpectre using case studies on several representative SGX binaries. Our evaluation shows that PowSpectre can exfiltrate unintended secrets in enclaves with very high accuracy. We perform a gadget analysis in SGX libraries and identify widely-existing code patterns that are power differentiable for PowSpectre. Our work highlights the need to synergistically understand the impact of speculation security with the introduction of new hardware functionalities.

[Download slides here](../files/powspectre_slides.pdf)

[Download paper here](../files/powspectre.pdf)

Recommended citation: M. H. I. Chowdhuryy, Z. Zhang, and F. Yao, “Powspectre: Powering up speculation attacks with tsx-based replay,” in ACM ASIACCS, 2024.