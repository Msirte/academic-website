---
title: Image-grade LiDAR Point Cloud Processing for Vegetation Monitoring
summary: This work focuses on processing vegetation point cloud data collected by image-grade LiDAR using image processing techniques. By leveraging depth priors from natural images, the method enables denoising and tail artifact removal in dense point clouds, thereby improving the quality and reliability of vegetation structure analysis.
tags:
  - Image Processing
date: '2025-05-03T00:00:00Z'

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
  
Traditional LiDAR point cloud processing methods typically rely on neighborhood-based operations and statistical filtering. However, dense point clouds—especially those captured by image-grade LiDAR—contain richer detail and implicit semantic information. This enables the application of image processing algorithms to point cloud denoising and tail artifact removal by effectively leveraging prior semantic knowledge.

Fig.1 illustrates the denoising performance of a variational PDE method based on total variation (TV) priors applied to dense vegetation point clouds.

<figure>
 <img src="fig1.jpg" alt="a" width="600px" height="600px"/>
  <figcaption>
      <h10>Fig. 1. TV denoising algorithm for dense pointcloud.</h10>
  </figcaption>
</figure>

</h8>