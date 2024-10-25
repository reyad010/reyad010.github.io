---
title: "LADDER: Architecting Content and Location-aware Writes for Crossbar Resistive Memories"
collection: publications
category: conferences
istop: yes
permalink: /publication/6/1/2022-ladder
excerpt: 'Resistive memories (ReRAM) organized in the form of crossbars are promising for main memory integration. While offering high cell density, crossbar-based ReRAMs suffer from variable write latency requirement for RESET operations due to the varying impact of IR drop, which jointly depends on the data pattern of the crossbar and the location of target cells being RESET. The exacerbated worst-case RESET latencies can significantly limit system performance. In this paper, we propose LADDER, an ...'
date: 6/1/2022
venue: 'IEEE/ACM International Symposium on Microarchitecture (MICRO)'
slidesurl: '../files/ladder_slides.pdf'
paperurl: '../files/ladder.pdf'
citation: 'M. H. I. Chowdhuryy, M. R. H. Rashed, A. Awad, R. Ewetz, and F. Yao, “Ladder: Architecting content and location-aware writes for crossbar resistive memories,” in IEEE MICRO, 2021.'
---
Resistive memories (ReRAM) organized in the form of crossbars are promising for main memory integration. While offering high cell density, crossbar-based ReRAMs suffer from variable write latency requirement for RESET operations due to the varying impact of IR drop, which jointly depends on the data pattern of the crossbar and the location of target cells being RESET. The exacerbated worst-case RESET latencies can significantly limit system performance. In this paper, we propose LADDER, an effective and low-cost processor-side framework that performs writes with variable latency by exploiting both content and location dependencies. To enable content awareness, LADDER incorporates a novel scheme that maintains metadata for per-row data pattern (i.e., number of 1’s) in memory, and performs efficient metadata management and caching through the memory controller. LADDER does not require hardware changes to the ReRAM chip. We design several optimizations that further boost the performance of LADDER, including LRS-metadata estimation that eliminates stale memory block reads, intra-line bit-level shifting that reduces the worst-case LRS-counter values and multi-granularity LRS-metadata design that optimizes the number of counters to maintain. We evaluate the efficacy of LADDER using 16 single- and multi-programmed workloads. Our results show that LADDER exhibits on average 46% performance improvement as compared to a baseline scheme and up to 33% over state-of-the-art designs. Furthermore, LADDER achieves 28.8% average dynamic memory energy saving compared to the existing architecture schemes and has less than 3% impact on device lifetime.

[Download slides here](../files/ladder_slides.pdf)

[Download paper here](../files/ladder.pdf)

Recommended citation: M. H. I. Chowdhuryy, M. R. H. Rashed, A. Awad, R. Ewetz, and F. Yao, “Ladder: Architecting content and location-aware writes for crossbar resistive memories,” in IEEE MICRO, 2021.