---
title: "BeKnight: Guarding Against Information Leakage in Speculatively Updated Branch Predictors"
collection: publications
category: conferences
istop: yes
series: ICCAD'23
permalink: /publication/2/1/2023-beknight
excerpt: 'Information leakage through processor microarchi-tectural components exploiting speculative execution is raising significant security concerns. Modern commercial processors incorporate branch predictor designs where internal states of branch predictor structures are speculatively updated. Recent studies have shown that speculatively updated branch predictors allow side channel exploitation in the speculative domain, extending branch predictors to be another source of transmitting medium in ...'
date: 2/1/2023
venue: 'IEEE/ACM International Conference on Computer Aided Design (ICCAD)'
slidesurl: '../files/beknight_slides.pdf'
paperurl: '../files/beknight.pdf'
citation: 'M. H. I. Chowdhuryy, Z. Zhang, and F. Yao, “Beknight: Guarding against information leakage in speculatively updated branch predictors,” in IEEE ICCAD, 2023.'
---
Information leakage through processor microarchi-tectural components exploiting speculative execution is raising significant security concerns. Modern commercial processors incorporate branch predictor designs where internal states of branch predictor structures are speculatively updated. Recent studies have shown that speculatively updated branch predictors allow side channel exploitation in the speculative domain, extending branch predictors to be another source of transmitting medium in transient execution attacks. While postponing updates of branch predictor states at a later time (e.g., during commit) can avoid exploitation in the speculation domain, it can result in belated correction of prediction outcomes (e.g., branch direction), leading to non-trivial degradation of prediction performance. In this paper, we present BeKnight, a secure branch predictor design that defeats speculative side channels targeting the branch direction prediction structure as the source of leakage. BeKnight aims to retain the performance advantage of early branch predictor updates (i.e., at resolution time) while ensuring no transient leakage. To achieve this, BeKnight conscientiously tracks the own-ership and speculative changes of potentially unsafe pattern history entries using a small Speculative Pattern Lookaside Buffer (SPLB). BeKnight efficiently audits the use of pattern history by allowing subsequent predictions in the same domain to benefit from early updates while annulling potential leakage through ensuring architecturally correct pattern is used on detection of a domain conflict. We evaluate the performance of BeKnight using 24 representative workloads from SPEC-2017. Notably, BeKnight achieves almost identical performance compared to the system with insecure but performant speculatively-updated predictors.

[Download slides here](../files/beknight_slides.pdf)

[Download paper here](../files/beknight.pdf)

Recommended citation: M. H. I. Chowdhuryy, Z. Zhang, and F. Yao, “Beknight: Guarding against information leakage in speculatively updated branch predictors,” in IEEE ICCAD, 2023.