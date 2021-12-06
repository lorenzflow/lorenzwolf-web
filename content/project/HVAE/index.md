---
title: VAE on Hilbert Spaces to generate functional data
summary: My MSc thesis project with slides for a related talk I gave at a seminar.
tags:
- Functional Data Analysis
- Generative Models
- Variational Auto Encoder
date: "2021-12-02T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: VAE on Hilbert spaces to generate functional data.
  focal_point: Smart

links:
# - icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
# url_code: ""
# url_pdf: ""
# url_slides: ""
# url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

Generative models are attracting a lot of attention partly because of their ability to learn from cheap unlabelled data. 
Instead of learning to discriminate between categories or performing regression tasks, this class of models learns to generate synthetic samples 
with the same properties as the input data $ \mathbf{X} $ . More specifically a generative model aims to learn the distribution $ p(\mathbf{X}) $ which the input data originates from.
This enables us to understand the distribution of the data, synthesise data from this distirbution, and perform tasks such as:
- Augmenting data sets for better model generalisation
- Out of distribution detection
- Density estimation

While deep learning and generative models have lead to many successes partly because of advances in available data and computational resources, 
we have also seen a big step in data collection methods. The increasing amount of high frequency data arising from fields such as finance and medicine motivates the
perspective of functional data analysis (FDA). The central assumption of FDA is that observations are treated as discretised functions rather than multivariate vectors. This approach leads to several advantages especially when the observations contain many function evaulations (i.e. very high dimensional vectors).

Motivated by these two observations, I explored the applicability of Variational Autoencoders to functional data by representing the functional data in a basis.
My full thesis can be downloaded {{< staticref "uploads/FDA_Thesis.pdf" "newtab" >}}here{{< /staticref >}} and slides for the talk {{< staticref "uploads/FDA_Slides.pdf" "newtab" >}}here{{< /staticref >}}.


