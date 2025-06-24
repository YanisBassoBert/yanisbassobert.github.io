---
title: "Generative Binary Memory: Pseudo-Replay Class-Incremental Learning on Binarized Embeddings"
collection: publications
category: manuscripts
permalink: /publication/2025_generative_binary_memory
excerpt: 'We propose Generative Binary Memory (GBM), the first pseudo-replay method tailored for Binary Neural Networks in Class-Incremental Learning. Using Bernoulli Mixture Models, GBM generates compact binary samples and improves accuracy with less memory compared to state of the art.'
date: 2024-11-01
venue: 'ArXiv'
paperurl: 'https://arxiv.org/pdf/2503.10333'
citation: 'Basso-Bert, Y., Molnos, A., Lemaire, R., Guicquero, W., & Dupret, A. (2025). Generative Binary Memory: Pseudo-Replay Class-Incremental Learning on Binarized Embeddings. arXiv preprint arXiv:2503.10333.'
---
In dynamic environments where new concepts continuously emerge, Deep Neural Networks (DNNs) must adapt by learning new classes while retaining previously acquired ones. This challenge is addressed by Class-Incremental Learning (CIL). This paper introduces Generative Binary Memory (GBM), a novel CIL pseudo-replay approach which generates synthetic binary pseudo-exemplars. Relying on Bernoulli Mixture Models (BMMs), GBM effectively models the multi-modal characteristics of class distributions, in a latent, binary space. With a specifically-designed feature binarizer, our approach applies to any conventional DNN. GBM also natively supports Binary Neural Networks (BNNs) for highly-constrained model sizes in embedded systems. The experimental results demonstrate that GBM achieves higher than state-of-the-art average accuracy on CIFAR100 (+2.9%) and TinyImageNet (+1.5%) for a ResNet-18 equipped with our binarizer. GBM also outperforms emerging CIL methods for BNNs, with +3.1% in final accuracy and x4.7 memory reduction, on CORE50.