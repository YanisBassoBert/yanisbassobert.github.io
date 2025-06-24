---
title: "On Class-Incremental Learning for Fully Binarized Convolutional Neural Networks"
collection: publications
category: manuscripts
permalink: /publication/2024_paper_iscas
excerpt: 'TL;DR: We propose the first evaluation of incremental learning on a fully binary neural network (BNN), leveraging binary-only operations for efficient on-chip learning. Our custom-designed BNN reaches 53.3% accuracy on CIFAR-100 with just 4.1Mb of memory. We compare native and latent replay strategies under a class-incremental setup, revealing that latent replay outperforms native replay beyond a specific buffer size. Our binary model also maintains accuracy 10% higher than its full-precision equivalent over many retrainings, demonstrating strong robustness.'
date: 2024-05
venue: 'IEEE International Symposium on Circuits and Systems (ISCAS)'
slidesurl: 'http://academicpages.github.io/files/iscas_slides.pdf'
paperurl: 'https://ieeexplore.ieee.org/xpl/conhome/10557746/proceeding'
citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
Recent advances in Binary Neural Networks (BNNs) are opening up new possibilities for disruptive hardware accelerators. This paper extends prior work on incremental learning to BNNs, by proposing a specifically-designed fully-binarized net-work and evaluating it on two learning variants, i.e., native and latent replay. The proposed BNN achieves a 53.3% test accuracy on the CIFAR-100 benchmark while relying on a binary-only arithmetic, for a 4.1Mb model size. Given a class-incremental learning experimental setup, we evaluate the influence of replay buffer size on the strategy, highlighting a turning point where latent replay offers a better classification performance than Native replay. In addition, our approach exhibits robustness against a large number of successive retrainings with an accuracy always 10% higher than a full-precision counterpart.
