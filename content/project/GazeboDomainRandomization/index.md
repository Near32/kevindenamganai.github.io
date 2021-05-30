---
title: GazeboDomainRandomization
summary: "This is an implementation of some Domain Randomization tools within the ROS+Gazebo framework, following the work of Tobin et al. "Domain Randomization for Transferring Deep Neural Networks from Simulation to the Real Worl"."
tags:
- Unsupervised Learning
# date: "2019-06-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: "https://github.com/Near32/GazeboDomainRandomization"

image:
  caption: Example application
  focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/KeviDenam
# url_code: ""
# url_pdf: ""
# url_slides: ""
# url_video: ""
 
# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: ""
---

This is an implementation of some Domain Randomization tools within the ROS+Gazebo framework, following the work of Tobin et al. "Domain Randomization for Transferring Deep Neural Networks from Simulation to the Real Worl".

It can be used to generate virtual datasets for an object recognition task of your choice, as it will automatically generate the bounding boxes for the object we seek to recognize in every generated pictures. The object has to be rendered in a .dae file compatible with Gazebo, first.
