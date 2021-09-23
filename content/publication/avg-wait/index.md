+++

featured = true

# Project title.
title = "High-Priority Expected Waiting Times in the Delayed Accumulating Priority Queue with Applications to Health Care KPIs"

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
abstract = "We provide the first analytical expressions for the expected waiting time of high- priority customers in the delayed APQ by exploiting a classical conservation law for work-conserving queues. Additionally, we describe an efficient algorithm for exactly computing the expected waiting times of both low-priority and high-priority customers, requiring only the truncation of sums that converge exponentially quickly. These insights are used to demonstrate how the accumulation rate and delay level should be chosen by health care practitioners to optimize common key performance indicators (KPIs). In particular, we demonstrate that for certain nontrivial KPIs, an accumulating priority queue with a delay of zero is always preferable. Finally, we present a detailed investigation of the quality of an exponential approximation to the high-priority waiting time distribution, which we use to optimize the choice of queueing parameters with respect to both classes' waiting time distributions."

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