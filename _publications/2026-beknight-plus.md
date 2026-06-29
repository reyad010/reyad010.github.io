---
title: "BeKnight+: Mitigating Information Leakage in Speculatively-updated Branch Predictor"
collection: publications
category: manuscripts
istop: istop
series: TCAD'26
authors: Chowdhuryy, Md Hafizul Islam and Zhang, Zhenkai and Yao, Fan
year: 2026
permalink: /publication/6/1/2026-beknight-plus
excerpt: 'Information leakage through processor microarchitectural components exploiting speculative execution is raising significant security concerns. Modern commercial processors incorporate branch predictor designs where internal states of branch predictor structures are speculatively updated, which recent studies have shown to enable side channel exploitation in the speculative domain. In this work, we present BeKnight+, a secure branch predictor design that defeats speculative side channels targeting the branch direction prediction structure while retaining the performance advantage of early branch predictor updates ...'
date: 6/1/2026
venue: 'IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems (TCAD)'
paperurl: '/files/papers/beknight-plus.pdf'
citation: 'M. H. I. Chowdhuryy, Z. Zhang, and F. Yao, “BeKnight+: Mitigating information leakage in speculatively-updated branch predictor,” IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems (TCAD), 2026.'
---
<!-- TODO: replace the placeholder abstract below with the final journal abstract, and drop the camera-ready PDF at /files/papers/beknight-plus.pdf -->
Information leakage through processor microarchitectural components exploiting speculative execution is raising significant security concerns. Modern commercial processors incorporate branch predictor designs where internal states of branch predictor structures are speculatively updated. Recent studies have shown that speculatively updated branch predictors allow side channel exploitation in the speculative domain, extending branch predictors to be another source of transmitting medium in transient execution attacks. While postponing updates of branch predictor states at a later time (e.g., during commit) can avoid exploitation in the speculation domain, it can result in belated correction of prediction outcomes (e.g., branch direction), leading to non-trivial degradation of prediction performance. In this paper, we present BeKnight+, a secure branch predictor design that defeats speculative side channels targeting the branch direction prediction structure as the source of leakage. BeKnight+ aims to retain the performance advantage of early branch predictor updates (i.e., at resolution time) while ensuring no transient leakage. To achieve this, BeKnight+ conscientiously tracks the ownership and speculative changes of potentially unsafe pattern history entries using a small Speculative Pattern Lookaside Buffer (SPLB). BeKnight+ efficiently audits the use of pattern history by allowing subsequent predictions in the same domain to benefit from early updates while annulling potential leakage through ensuring architecturally correct pattern is used on detection of a domain conflict.

[Download paper here](/files/papers/beknight-plus.pdf)

Recommended citation: M. H. I. Chowdhuryy, Z. Zhang, and F. Yao, “BeKnight+: Mitigating information leakage in speculatively-updated branch predictor,” IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems (TCAD), 2026.
