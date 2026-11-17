---
title: "CSC: Turning the Adversary's Poison against Itself"
collection: publications
category: conferences
permalink: /publication/2026-07-01-csc-turning-adversarys-poison-against-itself
date: 2026-07-01
venue: '31st Australasian Conference on Information Security and Privacy (ACISP 2026, CCF-C)'
paperurl: 'https://link.springer.com/chapter/10.1007/978-981-92-3015-0_14'
bibtexurl: 'https://ycsek.github.io/files/bibtex-csc.bib'
citation: "Shi, Y., Guo, X., Chen, H., Zhu, T., Liu, B., & Zhou, W. (2026, July). CSC: Turning the Adversary’s Poison Against Itself. In Australasian Conference on Information Security and Privacy (pp. 303-323). Singapore: Springer Nature Singapore."
---

## Abstract

Poisoning-based backdoor attacks pose significant threats to deep neural networks by embedding triggers in training data, causing models to misclassify triggered inputs as adversary-specified labels while maintaining performance on clean data. Existing poison restraint-based defenses often suffer from inadequate detection against specific attack variants and compromise model utility through unlearning methods that lead to accuracy degradation.

This paper conducts a comprehensive analysis of backdoor attack dynamics during model training, revealing that poisoned samples form isolated clusters in latent space early on, with triggers acting as dominant features distinct from benign ones. Leveraging these insights, we propose Cluster Segregation Concealment (CSC), a novel poison suppression defense.

CSC first trains a deep neural network via standard supervised learning while segregating poisoned samples through feature extraction from early epochs, DBSCAN clustering, and identification of anomalous clusters based on class diversity and density metrics. In the concealment stage, identified poisoned samples are relabeled to a virtual class, and the model's classifier is fine-tuned using cross-entropy loss to replace the backdoor association with a benign virtual linkage, preserving overall accuracy.

CSC was evaluated on four benchmark datasets against twelve poisoning-based attacks, CSC outperforms nine state-of-the-art defenses by reducing average attack success rates to near zero with minimal clean accuracy loss. Contributions include robust backdoor patterns identification, an effective concealment mechanism, and superior empirical validation, advancing trustworthy artificial intelligence.
