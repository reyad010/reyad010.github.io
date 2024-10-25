---
title: "MetaLeak: Uncovering Side Channels in Secure Processor Architectures Exploiting Metadata"
collection: publications
category: conferences
istop: istop
series: ISCA'24
authors: Chowdhuryy, Md Hafizul Islam and Zheng, Hao and Yao, Fan
year: 2024
permalink: /publication/5/1/2024-metaleak
excerpt: 'Microarchitectural side channels raise severe security concerns. Recent studies indicate that microarchitecture security should be examined holistically (rather than separately) in systems. Although the effects of performance optimizations on side channels are widely studied, the impacts of integrating security mechanisms intended for other threats on microarchitecture security are not well explored. In this paper, we perform the first side channel exploration in secure processor architectures ...'
date: 5/1/2024
venue: 'IEEE/ACM Annual International Symposium on Computer Architecture (ISCA)'
slidesurl: '../files/metaleak_slides.pdf'
paperurl: '../files/metaleak.pdf'
citation: 'M. H. I. Chowdhuryy, H. Zheng, and F. Yao, “Metaleak: Uncovering side channels in secure memory architectures exploiting metadata,” in IEEE ISCA, 2024.'
---
Microarchitectural side channels raise severe security concerns. Recent studies indicate that microarchitecture security should be examined holistically (rather than separately) in systems. Although the effects of performance optimizations on side channels are widely studied, the impacts of integrating security mechanisms intended for other threats on microarchitecture security are not well explored. In this paper, we perform the first side channel exploration in secure processor architectures that offer data confidentiality and integrity protection through hardware. We investigate microarchitecture security in the design space of secure processors and identify unique properties in the underlying metadata management schemes, which can be leveraged for new information leakage attacks. We present MetaLeak, an end-to-end side channel attack framework that exploits timing variations due to metadata maintenance to exfiltrate program secrets in secure processors. Particularly, we present two variants of the attack: MetaLeak-T that exploits the sharing of integrity tree metadata, and MetaLeak-C that manipulates counter metadata states. Our evaluation first shows highly accurate covert communication using the security metadata that can operate across cores and sockets without explicit data sharing. We further perform extensive side channel case studies on state-of-the-art secure architecture designs as well as the SGX processors. Our results show that MetaLeak can successfully exfiltrate program secrets (up to $97 \%$ accuracy) from image-processing application and cryptographic software running in enclave. Our study indicates that the fundamental metadata mechanism is the root cause of the leakage, which necessitates the use of leakage-taming techniques in future secure processors. This work highlights the need to synergistically understand microarchitecture security, as new security mechanisms are integrated.

[Download slides here](../files/metaleak_slides.pdf)

[Download paper here](../files/metaleak.pdf)

Recommended citation: M. H. I. Chowdhuryy, H. Zheng, and F. Yao, “Metaleak: Uncovering side channels in secure memory architectures exploiting metadata,” in IEEE ISCA, 2024.