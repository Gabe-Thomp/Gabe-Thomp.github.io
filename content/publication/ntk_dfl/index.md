---
title: 'NTK-DFL: Enhancing Decentralized Federated Learning in Heterogeneous Settings via Neural Tangent Kernel'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Kai Yue
  - Chau-Wai Wong
  - Huaiyu Dai 
# Author notes (optional)
author_notes: []

date: "2025-06-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: '2024-07-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: "In *Proceedings of the 42nd International Conference on Machine Learning*"
publication_short: "In *ICML*"

abstract: "Decentralized federated learning (DFL) is a collaborative machine learning framework for training a model across participants without a central server or raw data exchange. DFL faces challenges due to statistical heterogeneity, as participants often possess data of different distributions reflecting local environments and user behaviors. Recent work has shown that the neural tangent kernel (NTK) approach, when applied to federated learning in a centralized framework, can lead to improved performance. We propose an approach leveraging the NTK to train client models in the decentralized setting, while introducing a synergy between NTK-based evolution and model averaging. This synergy exploits interclient model deviation and improves both accuracy and convergence in heterogeneous settings. Empirical results demonstrate that our approach consistently achieves higher accuracy than baselines in highly heterogeneous settings, where other approaches often underperform. Additionally, it reaches target performance in 4.6 times fewer communication rounds. We validate our approach across multiple datasets, network topologies, and heterogeneity settings to ensure robustness and generalization."

# Summary. An optional shortened abstract.
summary: "This paper extends the neural tangent kernel training paradigm to decentralized federated learning (DFL). We discover a synergy that emerges from our approach in DFL. Our method encourages useful deviations between client models, improving overall generalization when models are aggregated."

tags:
  - Federated Learning
  - Decentralized Learning
  - Neural Tangent Kernel

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2410.01922'
url_code: 'https://github.com/Gabe-Thomp/ntk-dfl'
url_dataset: ''
url_poster: 'https://drive.google.com/file/d/1oPF6owFgdtjGVRBc_MGAqBtN-E-nTLd6/preview'
url_project: ''
url_slides: 'https://drive.google.com/file/d/1F1n2fm1d-dSwxziuE447t0hZWCI5Ofmi/view?usp=sharing'
url_source: 'https://arxiv.org/abs/2410.01922'
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image caption'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: "content/slides/ntk_slides.pdf"
---


{{% callout note %}}
I was fortunate enough to have the opportunity to present our work at ICML 2025 in Vancouver! ✈️✈️
{{% /callout %}}

## ICML Poster
I was fortunate enough to have the opportunity to present our work at ICML 2025 in Vancouver! ✈️✈️
![](poster.png "Here is the poster that I presented at ICML.")

## Non-technical Overview

*I find that much of academic writing is overly jargon-heavy and intimidating. Here I give a short description of the paper in a more accessible tone.*

**A short summary**:
Collaborative training of machine learning models is gaining traction as large, ChatGPT-like models take an unprecedented amount of computing resources to train. Particularly, individuals may want to collaboratively train models without explicitly sharing their personal data, and without the need for a larger, central server. In other words, models may be trained in a decentralized fashion.
This introduces the problem of data heterogeneity: different users have different kinds of data! Your mom may love pictures of cats, while your brother only takes pictures of dogs and parrots. If we were training an animal classifier on these images, the variation of data across devices can hinder training.  
In our paper, we investigate a training algorithm that replaces the typical training approach with a new one. We use a mathematical tool called the neural tangent kernel. In plain English, this tool allows the user to share more expressive data in the training process. By sharing better data, model training is enhanced despite the data variation discussed prior. Also, users must communicate with over fewer rounds than in previously proposed algorithms. Lastly, we provide open-source code for the research community to test and build upon our algorithm.

<!-- {{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}
 -->
Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
