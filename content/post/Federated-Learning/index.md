---
title: A future of Data Science and Machine Learning
subtitle: Is the hot topic of federated learning the solution to all our problems?

# Summary for listings and search engines
summary: A workshop the other week reminded me of federated learning, a hot topic in the ML community and in industry. 
          In this post I write about federated learning, the advantages and challenges and some exciting papers I came across.

# Link this post with a project
projects: []

# Date published
date: "2020-12-13T00:00:00Z"

# Date updated
lastmod: "2020-12-13T00:00:00Z"

# Is this an unpublished draft?
draft: true

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- Machine Learning

categories:
- Machine Learning
---

## Introduction

The other week I attended a workshop titled 'Interpretability, safety, and security in AI' hosted by The Alan Turing institute. 
Among many inspiring speakers, interesting talks, and exciting discussions (maybe I will write more about this in the next post, 
but the sessions were also recorded and will be on Youtube for those who feel like they missed out) 
one thing resonated with me in particular and reminded me of a topic I started reading about a while ago.

Isaac Kohane from Harvard University envisioned the future of healthcare 
as people owning their data and deciding when to put it to use and make it available to researchers. This idea of people being in control of their data is very exciting. 
It would put you and me in control of the information that is stored about us, whether it is health records, browsing history or finances. 
Being in control would mean that we could opt in to studies and allow researchers to access our relevant data to for example study a disease.
However, in the case of healthcare this is very sensitive information and as much as we might care about the cause we do not want to share our data for research purposes. 
Ultimately, the question is whether we trust whomever we allow to access our data.

This is a problem federated learning aims to address. In the following sections I write about the idea of federated learning, how it can be combined with tools from privacy, and some of the challenges that remain.

## Federated Learning Basics



