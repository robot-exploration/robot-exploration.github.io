---
title: "Network Localization Based Planning for Autonomous Underwater Vehicles with Inter-Vehicle Ranging"
authors:
- admin
- John Leonard
date: "2020-10-03T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2020-09-30T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *Autonomous Underwater Vehicles Symposium 2020*
publication_short: In *AUV 2020*

abstract: Localization between a swarm of AUVs can be entirely estimated through the use of range measurements between neighboring AUVs via a class of techniques commonly referred to as sensor network localization. However, the localization quality depends on network topology, with degenerate topologies, referred to as low-rigidity configurations, leading to ambiguous or highly uncertain localization results. This paper presents tools for rigidity-based analysis, planning, and control of a multi-AUV network which account for sensor noise and limited sensing range. We evaluate our long-term planning framework in several two-dimensional simulated environments and show we are able to generate paths in feasible time and guarantee a minimum network rigidity over the full course of the paths.

# Summary. An optional shortened abstract.
summary: Path-planning algorithm for networks of robots that use inter-robot distance measurements to localize

tags:
- Path Planning
featured: true

links:
- name: arXiv
  url: https://arxiv.org/abs/2010.02861
url_pdf: https://arxiv.org/pdf/2010.02861.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image by Alan Papalia'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

In many environments, such as underwater, it can be difficult to get reliable
localization using visual features. This could be due to the environment being highly repetitive or there being a general sparsity of features. In these situations the performance of traditional localization techniques tends to degrade and can give highly incorrect errors.

A key direction in my research is leveraging the use of inter-agent ranging, a
measurement which does not depend on environmental observation, to aid the
multi-robot localization task. However, there is a caveat, the quality of range-based localization varies based on the connectivity and spatial arrangement of the network of agents.

In this work I developed a planner which allowed for networks of agents to
efficiently plan trajectories that allowed them to stay in configurations which
were favorable for range-based localization. Read more about it <a href="https://arxiv.org/abs/2010.02861">
here</a>!



