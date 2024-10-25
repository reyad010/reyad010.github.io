---
title: "IvLeague: Side Channel-resistant Secure Architectures Using Isolated Domains of Dynamic Integrity Trees"
collection: publications
category: conferences
istop: yes
series: MICRO '21
permalink: /publication/11/1/2024-ivleague
excerpt: 'Modern secure processors rely on hardware-assisted encryption and tree-based integrity verification to protect off-chip data. However, despite extensive research on performance optimization, there is a significant lack of emphasis on side channel vulnerabilities in secure architectures. Given the strong focus on data security, it is critical to ensure that the integration of new design elements into secure architectures does not inadvertently introduce additional vulnerabilities. Existing ...'
date: 11/1/2024
venue: 'IEEE/ACM International Symposium on Microarchitecture (MICRO)'
slidesurl: '../files/ivleague_slides.pdf'
paperurl: '../files/ivleague.pdf'
citation: 'M. H. I. Chowdhuryy and F. Yao, “IvLeague: Side Channel-resistant Secure Architectures Using Isolated Domains of Dynamic Integrity Trees,” IEEE MICRO, 2024.'
---
Modern secure processors rely on hardware-assisted encryption and tree-based integrity verification to protect off-chip data. However, despite extensive research on performance optimization, there is a significant lack of emphasis on side channel vulnerabilities in secure architectures. Given the strong focus on data security, it is critical to ensure that the integration of new design elements into secure architectures does not inadvertently introduce additional vulnerabilities. Existing integrity verification mechanisms use a global integrity tree shared across security domains, which can introduce side channel leakage through integrity tree metadata sharing. In this work, we present IvLeague framework – a novel integrity verification mechanism for side channel-resistant isolated integrity trees among dynamic domains in secure processors. Specifically, IvLeague splits the global tree into multiple fixed-size subtrees, dynamically allocating these subtrees to domains during runtime. IvLeague enables efficient runtime scaling of memory coverage for individual domains. Additionally, we IvLeague-Invert, an optimization which shortens the integrity verification path by mapping data pages to high-level tree nodes. Finally, IvLeaguePro further improves the integrity verification of hotpages by enabling efficient hotpage tracking and migrating hotpages closer to the root. We extensively evaluate all three IvLeague schemes using 16 real-world workloads with varying memory footprints. IvLeague scheme, along with its optimizations, demonstrates a 5%-19% speedup over the insecure baseline, while providing effective side channel protection for the integrity tree. Moreover, IvLeague ensures high utilization of TreeLings (over 99.5%) and supports workloads with highly skewed memory footprints.

[Download slides here](../files/ivleague_slides.pdf)

[Download paper here](../files/ivleague.pdf)

Recommended citation: M. H. I. Chowdhuryy and F. Yao, “IvLeague: Side Channel-resistant Secure Architectures Using Isolated Domains of Dynamic Integrity Trees,” IEEE MICRO, 2024.