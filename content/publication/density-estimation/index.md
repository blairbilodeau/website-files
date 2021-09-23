+++

# Project title.
title = "Minimax Rates for Conditional Density Estimation via Empirical Entropy"

# Date this page was created.
date = 2021-06-01

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Blair Bilodeau", "Dylan J. Foster", "Daniel M. Roy"]

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
abstract = "We consider the task of estimating a conditional density using i.i.d. samples from a joint distribution, which is a fundamental problem with applications in both classification and uncertainty quantification for regression. For joint density estimation, minimax rates have been characterized for general density classes in terms of uniform (metric) entropy, a well-studied notion of statistical capacity. When applying these results to conditional density estimation, the use of uniform entropy -- which is infinite when the covariate space is unbounded and suffers from the curse of dimensionality -- can lead to suboptimal rates. Consequently, minimax rates for conditional density estimation cannot be characterized using these classical results. We resolve this problem for well-specified models, obtaining matching (within logarithmic factors) upper and lower bounds on the minimax Kullback--Leibler risk in terms of the empirical Hellinger entropy for the conditional density class. The use of empirical entropy allows us to appeal to concentration arguments based on local Rademacher complexity, which -- in contrast to uniform entropy -- leads to matching rates for large, potentially nonparametric classes and captures the correct dependence on the complexity of the covariate space. Our results require only that the conditional densities are bounded above, and do not require that they are bounded below or otherwise satisfy any tail conditions."

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
links = [{name = "Cite", url = "publication/density-estimation/cite.txt"},
        {name = "arXiv", url = "https://arxiv.org/abs/2109.10461"},
        {name = "Slides", url = "publication/density-estimation/slides.pdf"},
					{name = "Talk", url = "http://www.fields.utoronto.ca/talks/Minimax-Rates-Conditional-Density-Estimation-Empirical-Entropy"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
