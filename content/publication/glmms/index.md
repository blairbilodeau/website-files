+++

featured = true

# Project title.
title = "Fitting Generalized Linear Mixed Models using Adaptive Quadrature"

# Date this page was created.
date = 2022-02-01

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Alex Stringer<sup>*</sup>", "Blair Bilodeau<sup>*</sup>"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference Paper
# 2 = Journal Article
# 3 = Work in Progress
# 4 = Technical report
# 5 = Book
# 6 = Book chapter
publication_types = ["3"]

# Publication name and optional abbreviated version.
publication = "arXiv Preprint"
publication_short = "arXiv Preprint"

# Abstract.
abstract = "We describe how to approximate the intractable marginal likelihood that arises when fitting generalized linear mixed models. We prove that non-adaptive quadrature approximations yield high error asymptotically in every statistical model satisfying weak regularity conditions. We derive the rate of error incurred when using adaptive quadrature to approximate the marginal likelihood in a broad class of generalized linear mixed models, which includes non-exponential family response and non-Gaussian random effects distributions. We provide an explicit recommendation for how many quadrature points to use, and show that this recommendation recovers and explains many empirical results from published simulation studies and data analyses. Particular attention is paid to models for dependent binary and survival/time-to-event observations. Code to reproduce results in the manuscript is found at https://github.com/awstringer1/glmm-aq-paper-code."

# Project summary to display on homepage.
summary = ""

# Digital Object Identifier (DOI)
doi = ""

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references 
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects = []

# Optional external URL for project (replaces project detail page).
external_link = ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides = ""

# Links (optional).
url_preprint = ""
url_poster = ""
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
links = [{name = "Cite", url = "publication/glmms/cite.txt"},
        {name = "arXiv", url = "https://arxiv.org/abs/2202.07864"},
        {name = "Code", url = "https://github.com/awstringer1/glmm-aq-paper-code"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
