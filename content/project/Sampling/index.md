---
title: MCMC and some Variations
summary: I implemented and compared standard MCMC with MCMC using an adaptive proposal distribution. Furthermore, I implemented and analysed parallel tempering to sample from a bimodal distribution.

tags:
- MCMC
- Adaptive MCMC
- Parallel Tempering
date: "2021-12-02T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Sampled data points
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

Markoc Chain Monte Carlo (MCMC) is a powerful tool to approximate high dimensional intractable integrals, as for example often required for Bayesian inference. It allows the approximation of intractible integrals as well as sampling from an intractible distribution. A common challenge with MCMC is the choice of the proposall distribution, as this critically affects the mixing of the change and consequently the quality of any approximations deduced from the samples. We need to find a balance between good mixing and computational efficiency to quickly sample from the proposal. With increasing dimensionality tuning the proposal distribution becomes harder and harder which lead to the suggestion of adaptive proposal distributions. [Haario et al.](https://link.springer.com/article/10.1007/s001800050022) proposed such an algorithm adjusting the proposal distribution based on the already obtained samples. 

In the first part I implemented and compared the standard MCMC and the adaptive MCMC for the following density on $\mathbb{R}^{2}$
$$f(x, y) = k * \exp \left(-\frac{x^{2}}{100}-\left(y+\frac{3}{100} x^{2}-3\right)^{2}\right).$$

Summarising the results, the adaptive proposal performed better with the key aspects being:
- Increased computational efficiency
- Faster convergence and less dependence in the chain
- Higher effective sample size
- Samples are more representative of true density especially in the tails of the distribution

Another challenge is multimodality. With the wrong proposal distribution we may only capture the dominant mode or the chain can be become very sticky. One way to address this issue is tempering. In the second part I compared an additive random walk metropols hastings algorithm with a parallel tempering scheme.

The full project report including code can be downloaded here {{< staticref "uploads/Sampling/report.pdf" "newtab" >}}here{{< /staticref >}}.

