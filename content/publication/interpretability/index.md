+++

# Project title.
title = "Impossibility Theorems for Feature Attribution"

# Date this page was created.
date = 2024-01-05

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Blair Bilodeau", "Natasha Jaques", "Pang Wei Koh", "Been Kim"]

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
publication = "Proceedings of the National Academy of Sciences"
publication_short = "Proceedings of the National Academy of Sciences"

# Abstract.
abstract = "Despite a sea of interpretability methods that can produce plausible explanations, the field has also empirically seen many failure cases of such methods. In light of these results, it remains unclear for practitioners how to use these methods and choose between them in a principled way. In this paper, we show that for even moderately rich model classes (easily satisfied by neural networks), any feature attribution method that is complete and linear--for example, Integrated Gradients and SHAP--can provably fail to improve on random guessing for inferring model behaviour. Our results apply to common end-tasks such as identifying local model behaviour, spurious feature identification, and algorithmic recourse. One takeaway from our work is the importance of concretely defining end-tasks. In particular, we show that once such an end-task is defined, a simple and direct approach of repeated model evaluations can outperform many other complex feature attribution methods."

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
links = [{name = "Cite", url = "publication/interpretability/cite.txt"},
        {name = "arXiv", url = "https://arxiv.org/abs/2212.11870"},
        {name = "Poster", url = "publication/interpretability/poster.pdf"},
        {name = "Code", url = "https://github.com/google-research/interpretability-theory"},
        {name = "Published Version", url = "https://www.pnas.org/doi/10.1073/pnas.2304406120"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
