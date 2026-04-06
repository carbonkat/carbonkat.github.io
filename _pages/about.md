---
layout: page
title: About
permalink: /about/

carousels:
  - images: 
    - image: ../images/velcro_concept.png
    - image: ../images/velcro_architecture.png
    - image: ../images/ex_1.png
    - image: ../images/ex_2.png
    - image: ../images/ex_3.png
  - images: 
    - image: ../images/hex_framework.png
    - image: ../images/hex_factual_ex_1.png
    - image: ../images/hex_cf_ex_2.png
---

## Under Construction

## Research Interests

### Multi-Modal Learning
<img src="../images/personal_website_multimodal_img.png" width="25%">

I am passionate about advancing translational deep learning research in the medical domain, with a particular focus on multi-modal machine learning. My work centers on designing AI models that, much like human clinicians, can synthesize information from diverse sources such as laboratory tests, medical images, patient histories, and genetic data. By developing methods that enable models to effectively integrate and interpret heterogeneous data, I aim to contribute to more holistic and personalized healthcare solutions. My interest is driven by the belief that leveraging advanced multi-modal learning techniques can lead to more comprehensive patient insights and ultimately improve clinical decision-making.

### Trustworthy AI
<img src="../images/XAI.png" width="25%">

My research interests also include developing explainable and trustworthy AI for clinical applications. As deep learning models become more prevalent in healthcare delivery, I am committed to ensuring that the decisions these systems make are both accurate and interpretable to end users. My work emphasizes the integration of robust explainability mechanisms into model workflows to help medical practitioners understand, trust, and effectively use AI-based insights in their decision-making processes. By prioritizing ethical model design and deployment, my goal is to bridge the gap between complex machine learning systems and real-world clinical use.

#### Concept-Oriented Explanations

#### Encouraging Warranted Trust

## Selected Projects

### Visual Entity Linking with Contrastive Region-of-Interest Alignment (VELCRO)

{% include carousel.html height="50" unit="%" duration="20" number="1" %}

> [Read the paper!](https://openreview.net/pdf?id=84W63lKyRG)

The medical domain generates large amounts of imaging data every day. These images contain a wealth of knowledge about human health, but that information is only useful if extracted through successful analysis by domain experts. To keep pace with this ever-increasing flow, tools that assist users with a variety of image processing tasks, such as information retrieval and database management, are needed now more than ever. 

AI-assisted image analysis is a promising solution. In specialized domains, however, these tasks are most useful when images are explicitly connected to domain knowledge, allowing AI to better understand the semantics of image content. This can be achieved through an intermediate knowledge extraction step during processing, called visual entity linking (VEL). In VEL, salient entities in images are identified and grounded in a structured knowledge base (KB). This project focused specifically on targeted visual-to-textual entity linking (targeted V2TEL) to support user-guided tasks. This accounts for the fact that not all entities in a given image may be necessary to respond to a user’s information need and thus do not need to be linked.

In this project, KB entities were represented as text descriptions, making direct comparisons with the information represented in images challenging. To bridge this gap, information must be translated between modalities by condensing them into embeddings that can be projected into a shared latent space. With contrastive learning, models can be trained to learn to create and align image and text embeddings within this latent space such that semantically similar embeddings are close and semantically different ones are far apart. Once in the same space, entity linking reduces to a cosine similarity comparison between embeddings.

Following previous cross-modal alignment work such as CLIP, our VEL model, VELCRO, uses a two-tower architecture consisting of two submodels, each dedicated to processing a single modality (visual input or entities). To incorporate user intent, the visual tower also includes a visual prompt to ensure that only embeddings of the desired visual mentions are produced for linking. To address context challenges, the resulting embedding highlights the user’s target entity while still capturing information from its surroundings.


### Hierarchical Explanations (HEX)

{% include carousel.html height="50" unit="%" duration="20" number="2" %}

> Publicly available paper coming soon!

### RibXpert
