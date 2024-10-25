---
title: "D-Shield: Enabling Processor-side Encryption and Integrity Verification for Secure NVMe Drives"
collection: publications
category: conferences
istop: istop
series: HPCA'23
authors: Chowdhuryy, Md Hafizul Islam and Jung, Myoungsoo and Yao, Fan and Awad, Amro
year: 2023
permalink: /publication/6/1/2023-d-shield
excerpt: 'Ensuring the confidentiality and integrity of data stored in storage disks is essential to protect users’ sensitive and private data. Recent developments of hardware-based attacks have motivated the need to secure storage data not only at rest but also in transit. Unfortunately, existing techniques such as software-based disk encryption and hardware-based self-encrypting disks fail to offer such comprehensive protection in today’s adversarial settings. With the advances of NVMe SSDs promising ...'
date: 6/1/2023
venue: 'IEEE International Symposium on High-Performance Computer Architecture (HPCA)'
slidesurl: '../files/d-shield_slides.pdf'
paperurl: '../files/d-shield.pdf'
citation: 'M. H. I. Chowdhuryy, M. Jung, F. Yao, and A. Awad, “D-shield: Enabling processor-side encryption and integrity verification for secure nvme drives,” in IEEE HPCA, 2023.'
---
Ensuring the confidentiality and integrity of data stored in storage disks is essential to protect users’ sensitive and private data. Recent developments of hardware-based attacks have motivated the need to secure storage data not only at rest but also in transit. Unfortunately, existing techniques such as software-based disk encryption and hardware-based self-encrypting disks fail to offer such comprehensive protection in today’s adversarial settings. With the advances of NVMe SSDs promising ultralow I/O latencies and high parallelism, architecting a storage subsystem that ensures the security of data storage in fast disks without adversely sacrificing their performance is critical.In this paper, we present D-Shield, a processor-side secure framework to holistically protect NVMe storage data confidentiality and integrity with low overheads. D-Shield integrates a novel DMA Interception Engine that allows the processor to perform security metadata maintenance and data protection without any modification to the NVMe protocol and NVMe disks. We further propose optimized D-Shield schemes that minimize decryption/re-encryption overheads for data transfer crossing security domains and utilize efficient in-memory caching of storage metadata to further boost system performance. We implement D-Shield prototypes and evaluate their efficacy using a set of synthetic and real-world benchmarks. Our results show that D-Shield can introduce up to 17× speedup for I/O intensive workloads compared to software-based protection schemes. For server-class database and graph applications, D-Shield achieves up to 96% higher throughput over software-based encryption and integrity checking mechanisms, while providing strong security guarantee against off-chip storage attacks. Meanwhile, D-Shield shows only 6% overhead on effective performance on real-world workloads and has modest in-storage metadata overhead and on-chip hardware cost.

[Download slides here](../files/d-shield_slides.pdf)

[Download paper here](../files/d-shield.pdf)

Recommended citation: M. H. I. Chowdhuryy, M. Jung, F. Yao, and A. Awad, “D-shield: Enabling processor-side encryption and integrity verification for secure nvme drives,” in IEEE HPCA, 2023.