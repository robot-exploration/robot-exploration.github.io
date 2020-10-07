---
title: Inter-Mobile-Device Distance Estimation using Network Localization Algorithms for Digital Contact Logging Applications
authors:
- Lillian Clark
- admin
- Jonata Tyska Carvalho
- Luca Mastrostefano
- Bhaskar Krishnamachari
date: "2020-07-20T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2020-09-30T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "In *Connected Health: Applications, Systems and Engineering Technologies*"
publication_short: "In *CHASE 2020*"

abstract: Mobile applications are being developed for automated logging of contacts via Bluetooth to help scale up digital contact tracing efforts in the context of the ongoing COVID-19 pandemic. A useful component of such applications is inter-device distance estimation, which can be formulated as a network localization problem. We survey several approaches and evaluate the performance of each on real and simulated Bluetooth Low Energy (BLE) measurement datasets with respect to both distance estimate accuracy and the proximity detection problem. We investigate the effects of obstructions like pockets, differences between device models, and the environment (i.e. indoors or outdoors) on performance. We conclude that while direct estimation can provide the best proximity detection when Received Signal Strength Indicator (RSSI) measurements are available, network localization algorithms like Isomap, Local Linear Embedding, and the spring model outperform direct estimation in the presence of missing or very noisy measurements. The spring model consistently achieves the best distance estimation accuracy. 

# Summary. An optional shortened abstract.
summary: Contact tracing techniques for devices with Bluetooth Low-Energy (BLE) measurements

tags:
- COVID-19
featured: false

links:
- name: arXiv
  url: https://arxiv.org/abs/2007.10162
url_pdf: https://arxiv.org/pdf/2007.10162.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: Figure by Lilly Clark
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

Most modern day phones are equipped with hardware that allows for Bluetooth
Low-Energy (BLE) communication with other phones. This can also be used to get a
rough distance between two phones, something which many teams have tried to use
to get contact tracing information. However, this approach has proven
challenging, with the measurements being highly noisy and there being a good
chance of two phones not having a measurement despite being within sensing range
of each other.

To try to combat these challenges, the contact tracing problem can be considered
a sensor network localization problem. This is a long-studied class of
algorithms which attempt to localize members of a network using only pairwise
distance measurements between network members. Modeling contact tracing as a
network localization problem serves two distinct benefits. First, this allows
for multiple measurements to be used to try to estimate the distance between
phones, combatting the effects of noisy data. Secondly, this allows for the
distance between two phones to be estimated even if there is no corresponding
distance measurement between these two devices.

In this collaboration I worked with <a
href="https://sites.google.com/usc.edu/lillyclark">Lilly Clark </a> to test out
a number of sensor network localization approaches for contact tracing. See our
results and read more about it <a href="https://arxiv.org/abs/2007.10162">
here</a>!

