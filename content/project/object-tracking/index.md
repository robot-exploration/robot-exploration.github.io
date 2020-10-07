---
title: 6-DOF Object Tracking
summary: A system for automated data collection and off-line pose estimation for predetermined objects for robotic grasping testbed
tags:
- Robotics
date: "2020-09-30T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo from Oregon State University
  focal_point: Smart

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

This project was part of a few months I spent at the <a
href="https://robotics.oregonstate.edu/"> Collaborative Robotics and Intelligent
Systems Institute</a> of Oregon State University. I was part of an NSF Research
Experience for Undergrads, and my goal was to develop an automated system for
tracking an object.

The larger goal was to build an entire testbed which researchers could remotely
access and test robotic grasping algorithms on. My part of the project would
allow for quantitative statistics on the grasping experiments.

To approach the problem I developed a Python library that was capable of
interfacing with Intel RGB-D cameras and recording several image streams in
parallel. To then perform object tracking several state-of-the-art pose
estimation techniques were implemented and compared. The comparison showed
improved reliability and performance under occlusion for a <a
href="https://labicvl.github.io/docs/pubs/Aly_ECCV_2014.pdf"> Latent-Class Hough
Forest framework</a> developed at the Imperial College London.

During a grasping experiment the data capture was set to be automated by the
RGB-D cameras and the images were then post-processed by the chosen framework.
