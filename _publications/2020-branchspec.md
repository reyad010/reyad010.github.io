---
title: "BranchSpec: Information Leakage Attacks Exploiting Speculative Branch Instruction Executions"
collection: publications
category: conferences
istop: no
series: ICCD'20
permalink: /publication/2/1/2020-branchspec
excerpt: 'Recent studies on attacks exploiting processor hardware vulnerabilities have raised significant concern for information security. Particularly, transient execution attacks such as Spectre augment microarchitectural side channels with speculative executions that lead to exfiltration of secretive data not intended to be accessed. Many prior works have demonstrated the manipulation of branch predictors for triggering speculative executions, and thereafter leaking sensitive information through ...'
date: 2/1/2020
venue: 'IEEE International Conference on Computer Design (ICCD)'
slidesurl: '../files/branchspec_slides.pdf'
paperurl: '../files/branchspec.pdf'
citation: 'M. H. I. Chowdhuryy, H. Liu, and F. Yao, “BranchSpec: Information Leakage Attacks Exploiting Speculative Branch Instruction Executions,” in IEEE ICCD, 2020.'
---
Recent studies on attacks exploiting processor hardware vulnerabilities have raised significant concern for information security. Particularly, transient execution attacks such as Spectre augment microarchitectural side channels with speculative executions that lead to exfiltration of secretive data not intended to be accessed. Many prior works have demonstrated the manipulation of branch predictors for triggering speculative executions, and thereafter leaking sensitive information through processor microarchitectural components. In this paper, we present a new class of microarchitectural attack, called BranchSpec, that performs information leakage by exploiting state changes of branch predictors in speculative path. Our key observation is that, branch instruction executions in speculative path alter the states of branch pattern history, which are not restored even after the speculatively executed branches are eventually squashed. Unfortunately, this enables adversaries to harness branch predictors as the transmitting medium in transient execution attacks. More importantly, as compared to existing speculative attacks (e.g., Spectre), BranchSpec can take advantage of much simpler code patterns in victim&apos;s code base, making the impact of such exploitation potentially even more severe. To demonstrate this security vulnerability, we have implemented two variants of BranchSpec attacks: a side channel where a malicious spy process infers cross-boundary secrets via victim&apos;s speculatively executed nested branches, and a covert channel that communicates secrets through intentionally perturbing the branch pattern history structure via speculative branch executions. Our evaluation on Intel Skylake- and Coffee Lake-based processors reveals that these information leakage attacks are highly accurate and successful. To the best of our knowledge, this is the first work to reveal the information leakage threat due to speculative state update in branch predictor. Our studies further broaden the attack surface of processor microarchitecture, and highlight the needs for branch prediction mechanisms that are secure in transient executions.

[Download slides here](../files/branchspec_slides.pdf)

[Download paper here](../files/branchspec.pdf)

Recommended citation: M. H. I. Chowdhuryy, H. Liu, and F. Yao, “BranchSpec: Information Leakage Attacks Exploiting Speculative Branch Instruction Executions,” in IEEE ICCD, 2020.