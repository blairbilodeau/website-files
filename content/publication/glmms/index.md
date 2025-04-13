+++

# Project title.
title = "Asymptotics of Numerical Integration for Two-Level Mixed Models"

# Date this page was created.
date = 2025-04-01

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["<sup>(A)</sup>Blair Bilodeau", "Alex Stringer", "Yanbo Tang"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference Paper
# 2 = Journal Article
# 3 = Work in Progress
# 4 = Technical report
# 5 = Book
# 6 = Book chapter
publication_types = ["2"]

# Publication name and optional abbreviated version.
publication = "Bernoulli (to appear)"
publication_short = "Bernoulli (to appear)"

# Abstract.
abstract = "We study mixed models with a single grouping factor, where inference about unknown parameters requires optimizing a marginal likelihood defined by an intractable integral. Low-dimensional numerical integration techniques are regularly used to approximate these integrals, with inferences about parameters based on the resulting approximate marginal likelihood. For a generic class of mixed models that satisfy explicit regularity conditions, we derive the stochastic relative error rate incurred for both the likelihood and maximum likelihood estimator when adaptive numerical integration is used to approximate the marginal likelihood. We then specialize the analysis to well-specified generalized linear mixed models having exponential family response and multivariate Gaussian random effects, verifying that the regularity conditions hold, and hence that the convergence rates apply. We also prove that for models with likelihoods satisfying very weak concentration conditions that the maximum likelihood estimators from non-adaptive numerical integration approximations of the marginal likelihood are not consistent, further motivating adaptive numerical integration as the preferred tool for inference in mixed models. Code to reproduce the simulations in this paper is provided at https://github.com/awstringer1/aq-theory-paper-code."

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
        {name = "Code", url = "https://github.com/awstringer1/aq-theory-paper-code"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
