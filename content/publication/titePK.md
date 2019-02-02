+++
title = "Phase I dose-escalation trials with more than one dosing regimen"
date = 2018-11-23T00:00:00

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Burak Kürsad Günhan", "Sebastian Weber", "Abdelkader Seroutou", "Tim Friede"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference proceedings
# 2 = Journal
# 3 = Work in progress
# 4 = Technical report
# 5 = Book
# 6 = Book chapter
publication_types = ["3"]

# Publication name and optional abbreviated version.
publication = "Submitted for publication"
publication_short = ""

# Abstract and optional shortened version.
abstract = "Traditionally, phase I dose-escalation oncology trials are designed to find a dose at which an acceptable event rate of dose limiting toxicities (DLT) occur. However, nowadays the dosing regimen, which determines the timing of drug administration, is varied in addition to the drug amount itself; e.g. a weekly or daily schedule. Standard methods such as the Bayesian Logistic Regression Model do not directly allow for more than one dosing regimen to be evaluated, and hence ad-hoc approaches like dose re-scaling are used to make dosing regimens comparable. To avoid such ad-hoc approaches, we propose a new statistical model that uses pharmacokinetic (PK) principles to integrate varying dosing regimens. We propose to use a latent pseudo-PK, which uses the preplanned dosing regimen. We complement the pseudo-PK by an effect compartment which admits a delay between the PK and the actual effect, the occurrence of a DLT. The effect compartment measure is used as exposure measure and set directly proportional to the instantaneous hazard of the time-to-first DLT event process. The model is formulated using interpretable parameters which facilitates the specification of priors. Moreover, we derive from the time-to-event model metrics which enable escalation with overdose control. In a Monte Carlo simulation study, the proposed model displayed desirable performance in terms of investigated measures across a range of dose-toxicity profiles including single and varying dosing regimens. The proposed model is motivated and illustrated by a real-life example. The software to implement the proposed model (R and Stan code) is publicly available."
abstract_short = "."

# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename of your project in `content/project/`.
#   Otherwise, set `projects = []`.
projects = []

# Links (optional).
url_pdf = "https://arxiv.org/pdf/1811.09433.pdf"
url_code = "https://github.com/gunhanb/TITEPK_code"

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#url_custom = [{name = "Custom Link", url = "http://example.org"}]

# Does the content use math formatting?
math = true

# Does the content use source code highlighting?
highlight = true

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = ""
caption = ""

+++

