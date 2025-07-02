---
title: "Phd thesis: Replay strategies for incremental learning in fully-binary neural networks under memory constraints"
collection: publications
category: manuscripts
permalink: /publication/2025-thesis-manuscript
excerpt: "This thesis explores how Fully Binarized Neural Networks (FBNNs) can support incremental learning under extreme memory and energy constraints. By combining compact architectures with novel replay strategies, it enables smart sensors to learn continuously, efficiently, and on-device. <br/>
  <img src='/images/schema-manuscript-organisation.svg' alt='organisation schema' width='800'>"
date: 2025-04-01
citation: 'Basso-Bert, Y. Replay strategies for incremental learning in fully-binary neural networks under memory constraints.'
---
Here is my full thesis, available in open access ([download link]('https://yanisbassobert.github.io/files/thesis.pdf')):

<img src='/images/schema-manuscript-organisation.svg' alt='organisation schema' width='800'>

<iframe src="https://yanisbassobert.github.io/files/thesis.pdf#toolbar=0" width="100%" height="500px" style="border: none;"></iframe>

The rise of smart sensors has led to a growing need to deploy deep learning models close to the sensor, enabling always-on on-device inference, where models run permanently to support uninterrupted local processing. This approach reduces latency, bandwidth, and energy consumption — especially important in resource-constrained environments.

To meet these constraints, typically a few megabits of memory and a few milliwatts of power, models must be specifically designed for efficient execution. Binary Neural Networks (BNNs) have emerged as a promising solution, replacing the costly multiply-accumulate operations of conventional deep neural networks with efficient logic-gate-based arithmetic.

However, near-sensor inference also requires models to adapt over time, as new concepts may appear or evolve in the deployment environment. Incremental learning strategies enable this adaptability by allowing models to be retrained on new data while preserving past knowledge. Among the various techniques developed for incremental learning, replay methods, where past knowledge is retained or approximated through stored or generated data, are particularly effective.

Yet, training BNNs remains difficult due to their non-differentiable operations and limited expressiveness, as they rely on only two discrete values. These challenges are further compounded in incremental settings, where retraining must occur repeatedly. Moreover, conventional replay methods introduce additional memory requirements that conflict with the tight constraints of edge deployment.

This thesis investigates whether Fully Binarized Neural Networks (FBNNs) can support incremental learning under extreme memory and energy constraints, and how memory-efficient replay mechanisms can be designed to make this possible.

We adopt a progressive research methodology, exploring replay strategies increasingly embedded into the binary architecture to reduce memory usage, starting from native replay, through latent replay, and finally to pseudo-replay.

We first establish best practices for training compact FBNNs under incremental learning constraints. This includes:

- The design of a fully binary architecture,

- A semi-supervised pretraining protocol that enhances representation transferability,

- A detailed study of loss balancing,

- A comparison between native and latent replay under tight memory budgets.

These findings are validated on CIFAR-100 and extended to the CORE50 benchmark, where our 3Mb FBNN achieves accuracy comparable to larger real-valued networks.

Building on this foundation, we introduce Generative Binary Memory (GBM), a pseudo-replay method based on Bernoulli Mixture Models that generates synthetic binary exemplars from compact prototype representations. Two binarization modules extend GBM to non-binary networks. The method achieves state-of-the-art results on CIFAR-100 (+2.9%) and TinyImageNet (+1.5%) with a ResNet18 backbone. On FBNNs, GBM improves final accuracy by +3.1% on CORE50 while reducing memory usage by a factor of 4.7. An online, integer-only variant of GBM is also proposed to support real-time on-device adaptation.

This work demonstrates that FBNNs, when designed and trained with appropriate strategies, can support incremental learning while meeting the stringent requirements of embedded inference. It opens promising directions for deploying adaptive, low-power learning systems at the edge.