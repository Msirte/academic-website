---
title: Underwater lightsource simulation
summary: Monte Carlo simulation of lightsources in water
tags:
  - Optics
date: '2024-03-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
<h8 style="text-align: justify;">
This is an ongoing project. This page is just for showing the preliminary results and will be updated in the future.

Using the Monte Carlo method, we simulate the light intensity distribution of an underwater light source. Based on an approximation of the multiple scattering model, each step in the underwater light propagation process is treated as a random sampling event, and the spatial energy distribution is computed throughout the propagation. The final underwater light source image is obtained by calculating the statistical expectation. The simulation focuses on three key components: the light source, the transmission medium, and the detector.

As shown in Figure 1, the photon transport characteristics are described by the Point Spread Function (PSF). The $PSF(R,\theta,\varphi)$ represents the probability that a photon emitted ialong the $z+$ direction within a specific water environment will arrive at a point in spherical coordinates $(R,\theta,\varphi)$ and incident at an angle $(\theta',\varphi')$.

Leveraging the geometric symmetry relationships, the light intensity distribution image on the detector for a light source with angular intensity distribution $I(\alpha)$ can be computed as:
$$
L(R, \theta, \phi) = \int I(\alpha) \cdot \text{PSF}(R, \theta, \phi \mid \alpha) \, d\alpha
$$

<figure>
 <img src="fig1.png" alt="a" width="600px" height="600px"/>
  <figcaption>
      <h10>Fig. 1. Simulated underwater images at different ALs.</h10>
  </figcaption>
</figure>

<figure>
 <img src="fig2.png" alt="a" width="600px" height="600px"/>
  <figcaption>
      <h10>Fig. 2. Image enhancement results on benchmark dataset (with references baseline).</h10>
  </figcaption>
</figure>

<figure>
 <img src="fig3.png" alt="a" width="600px" height="600px"/>
  <figcaption>
      <h10>Fig. 3. Image enhancement results on benchmark dataset (without references baseline).</h10>
  </figcaption>
</figure>

</h8>