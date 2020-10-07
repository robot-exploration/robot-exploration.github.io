---
title: Mixed-Integer Model Predictive Control
summary: Mixed-integer program to perform path-planning with model predictive control for simplified 2-D quadrotor environment
tags:
- Robotics
date: "2020-09-30T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Image by Alan Papalia
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: GitHub
  url: https://github.com/alanpapalia/miqcp-planning

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

As part of MIT's course 16.413 I worked on a team to derive a model-predictive controller for a simulated quadrotor in a non-convex planning space. I used <a href="https://scip.zib.de/"> SCIP</a>, an open-source optimization software in conjunction with simplified quadrotor dynamics model to perform the path-planning subject to obstacle avoidance constraints.

Because objects could be placed arbitrarily within the environment, the planning problem was inherently non-convex. For this reason the problem was modeled as a mixed-integer problem.

In <a href="https://github.com/alanpapalia/miqcp-planning"> this repo</a> all of our work is shown in a Jupyter Notebook, along with a brief explanation of some relevant topics in optimization and a derivation of the quadrotor dynamics.
