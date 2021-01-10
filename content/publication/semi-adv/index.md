+++
# Project title.
title = "Relaxing the I.I.D. Assumption: Adaptively Minimax Optimal Regret via Root-Entropic Regularization"

# Date this page was created.
date = 2020-07-13

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Blair Bilodeau<sup>*</sup>", "Jeffrey Negrea<sup>*</sup>", "Daniel M. Roy"]

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
abstract = "We consider sequential prediction with expert advice when data are generated from distributions varying arbitrarily within an unknown constraint set. We quantify relaxations of the classical i.i.d. assumption in terms of these constraint sets, with i.i.d. sequences at one extreme and adversarial mechanisms at the other. The Hedge algorithm, long known to be minimax optimal in the adversarial regime, was recently shown to be minimax optimal for i.i.d. data. We show that Hedge with deterministic learning rates is suboptimal between these extremes, and present a new algorithm that adaptively achieves the minimax optimal rate of regret with respect to our relaxations of the i.i.d. assumption, and does so without knowledge of the underlying constraint set. We analyze our algorithm using the follow-the-regularized-leader framework, and prove it corresponds to Hedge with an adaptive learning rate that implicitly scales as the square root of the entropy of the current predictive distribution, rather than the entropy of the initial predictive distribution."

# Project summary to display on homepage.
summary = ""

# Digital Object Identifier (DOI)
doi = ""

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["Featured"]

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
links = [{name = "Cite", url = "publication/semi-adv/cite.txt"},
		 {name = "arXiv", url = "https://arxiv.org/abs/2007.06552"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
