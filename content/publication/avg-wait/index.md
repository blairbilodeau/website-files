+++
# Project title.
title = "Average Waiting Times in the Two-Class M/G/1 Delayed Accumulating Priority Queue"

# Date this page was created.
date = 2020-01-01

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Blair Bilodeau", "David A. Stanford"]

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
abstract = "Previously, Mojalal et al. (2019) gave an expression for the waiting time distribution of low priority customers in the Delayed Accumulating Priority Queue, but with no quantification of the effect on others in system. We provide an analytical expression for the expected waiting time of both high and low priority customers by exploiting a conservation law for work conserving queues. Our expression can be efficiently implemented numerically, requiring only the truncation of sums which converge exponentially quickly. This enables us to use common key performance indicators to demonstrate how the accumulation rate and delay level should be chosen by health care practitioners."

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
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
links = [{name = "Cite", url = "publication/avg-wait/cite.txt"},
		 {name = "arXiv", url = "https://arxiv.org/abs/2001.06054"},
		 {name = "Slides", url = "publication/avg-wait/slides.pdf"},
		 {name = "Code", url = "https://github.com/blairbilodeau/delayed-apq-avg-wait"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++