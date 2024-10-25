---
title: "Leaking Secrets Through Modern Branch Predictors in the Speculative World"
collection: publications
category: manuscripts
istop: istop
series: TC'21
authors: Chowdhuryy, Md Hafizul Islam and Yao, Fan
year: 2022
permalink: /publication/6/1/2021-branchspectre
excerpt: 'Transient execution attacks that exploit speculation have raised significant concerns in computer systems. Typically, branch predictors are leveraged to trigger mis-speculation in transient execution attacks. In this work, we demonstrate a new class of speculation-based attacks that targets the branch prediction unit (BPU). We find that speculative resolution of conditional branches (i.e., in nested speculation) alter the states of pattern history table (PHT) in modern processors, which are not ...'
date: 6/1/2021
venue: 'IEEE Transactions on Computers (TC)'
slidesurl: '../files/branchspectre_slides.pdf'
paperurl: '../files/branchspectre.pdf'
citation: 'M. H. I. Chowdhuryy and F. Yao, “Leaking secrets through modern branch predictor in the speculative world,” IEEE TC, 2021.'
---
Transient execution attacks that exploit speculation have raised significant concerns in computer systems. Typically, branch predictors are leveraged to trigger mis-speculation in transient execution attacks. In this work, we demonstrate a new class of speculation-based attacks that targets the branch prediction unit (BPU). We find that speculative resolution of conditional branches (i.e., in nested speculation) alter the states of pattern history table (PHT) in modern processors, which are not restored after the corresponding branches are later squashed. Such characteristic allows attackers to exploit the BPU as the secret transmitting medium in transient execution attacks. To evaluate the discovered vulnerability, we build a novel attack framework, BranchSpectre, that enables exfiltration of unintended secrets through observing speculative PHT updates (in the form of covert and side channels). We further investigate the PHT collision mechanism in the history-based predictor and the branch prediction mode transitions in Intel processors. Built upon such knowledge, we implement an ultra-high speed covert channel (BranchSpectre-cc) as well as two side channels (i.e., BranchSpectre-v1 and BranchSpectre-v2) that merely rely on BPU for mis-speculation trigger and secret inference in the speculative domain. Notably, BranchSpectre side channels can take advantage of much simpler code patterns than those used in Spectre attacks. We present an extensive BranchSpectre code gadget analysis on a set of popular real-world application code bases followed by a demonstration of side channel attack on OpenSSL. The evaluation results show substantially wider existence and higher exploitability of BranchSpectre code patterns in real-world software. Finally, we discuss several secure branch prediction mechanisms that can mitigate transient execution attacks exploiting modern branch predictors.

[Download slides here](../files/branchspectre_slides.pdf)

[Download paper here](../files/branchspectre.pdf)

Recommended citation: M. H. I. Chowdhuryy and F. Yao, “Leaking secrets through modern branch predictor in the speculative world,” IEEE TC, 2021.