---
title: "Game of Threads: Enabling Asynchronous Poisoning Attacks"
collection: publications
permalink: /publication/2020-03-01-game-of-threads
excerpt: 'Our attack influences training outcome---e.g., degrades model accuracy or biases the model towards an adversary-specified label---purely by scheduling asynchronous training threads in a malicious fashion. Since thread scheduling is outside the protections of modern trusted execution environments (TEEs), e.g., Intel SGX, our attack bypasses these protections even when the training set can be verified as correct.'
date: 2020-03-01
venue: 'ASPLOS'
paperurl: 'https://dl.acm.org/doi/10.1145/3373376.3378462'
citation: 'Jose Rodrigo Sanchez Vicarte, Benjamin Schreiber, Riccardo Paccagnella, and Christopher W. Fletcher. 2020. Game of Threads: Enabling Asynchronous Poisoning Attacks. In Proceedings of the Twenty-Fifth International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS ’20). Association for Computing Machinery, New York, NY, USA, 35–52. DOI:https://doi.org/10.1145/3373376.3378462'
---
<img src="https://dl.acm.org/userimages/na101/home/literatum/publisher/acm/classification/LinkedImages/reproducibility-types/artifacts_available/icon-small_201811200510.png" width="50" alt="artifact available badge"/>
<img src="https://dl.acm.org/userimages/na101/home/literatum/publisher/acm/classification/LinkedImages/reproducibility-types/artifacts_evaluated_functional/icon-small_201811200512.png" width="50" alt="artifact evaluated and functional badge"/>

As data sizes continue to grow at an unprecedented rate, machine learning training is being forced to adopt asynchronous algorithms to maintain performance and scalability. In asynchronous training, many threads share and update the model in a racy fashion to avoid costly inter-thread synchronization.

This paper studies the security implications of these codes by introducing asynchronous poisoning attacks. Our attack influences training outcome---e.g., degrades model accuracy or biases the model towards an adversary-specified label---purely by scheduling asynchronous training threads in a malicious fashion. Since thread scheduling is outside the protections of modern trusted execution environments (TEEs), e.g., Intel SGX, our attack bypasses these protections even when the training set can be verified as correct. To the best of our knowledge, this represents the first example where a class of applications loses integrity guarantees, despite being protected by enclave-based TEEs such as SGX.

We demonstrate both accuracy degradation and model biasing attacks on the CIFAR-10 image recognition task, trained on Resnet-style DNNs using an asynchronous training code published by Pytorch. We also perform proof-of-concept experiments to validate our assumptions on an SGX-enabled machine. Our accuracy degradation attacks are capable of returning a converged model to pre-trained accuracy or to some accuracy in between. Our model biasing attack can force the model to predict an adversary-specified label up to ~40% of the time on the CIFAR-10 validation set (whereas the un-attacked model's prediction rate towards any label is ~10%).

[Download paper here](https://dl.acm.org/doi/10.1145/3373376.3378462)

[Articaft available here](https://zenodo.org/record/3598009)

[github repository available here](https://github.com/jose-sv/hogwild_pytorch)
