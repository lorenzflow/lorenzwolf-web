---
title: Statistically Modelling the Spread of HIV
summary: Abrief description of my UROP with Dr Oliver Ratmann.
tags:
- Statistics
- Epidemiology
date: "2021-12-02T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Transmission Dynamics of HIV
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
slides: example
---

During the summer 2019 I joined Dr Oliver Ratmann for 2 months to conduct research on the spread of HIV. The project was funded by an EPSRC bursuary. 

We performed a phylogeographic analysis to assess the geographic transmission rates. At the core of the project was a continuous-time Markov model. We worked with the software packages Beast to run the MCMC and FigTree to visualise the results. To tackle the issue of a high dimensional space with many negligible transmissions we applied Bayesian Stochastic Search Variable Selection (BSSVS). We quickly ran into an unexpected computational problem, as Beast did not allow the input of an existing tree, which shifted the project into the implementation of a function hardcoding the Beast input XML from an existing tree. The core reference for this project was this [paper by Bbosa et al.](https://www.nature.com/articles/s41598-018-37458-x#:~:text=Phylogeographic%20analysis%20showed%20strong%20support,virus%20strains%20from%20the%20GP.).
