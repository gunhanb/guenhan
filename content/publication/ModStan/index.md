---
title: "Shrinkage Estimation for Dose–Response Modeling in Phase II Trials With Multiple Schedules"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Paul Meyvisch
- Tim Friede 


# Author notes (optional)


date: "2020-05-01T00:00:00Z"
doi: "10.1080/19466315.2020.1850519"

# Schedule page publish date (NOT publication's date).
publishDate: "2019-08-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In Statistics in Biopharmaceutical Research
publication_short: In Statistics in Biopharmaceutical Research

abstract: Recently, phase II trials with multiple schedules (frequency of administrations) have become more popular, for instance, in the development of treatments for atopic dermatitis. If the relationship of the dose and response is described by a parametric model, a simplistic approach is to scale doses from different schedules to a common unit and pool all rescaled doses. However, this approach ignores the potential heterogeneity in dose–response curves between schedules. A more reasonable approach is the partial pooling, that is, certain parameters of the dose–response curves are shared, while others are allowed to vary. Rather than using schedule-specific fixed-effects, we propose a Bayesian hierarchical model with random-effects to model the between-schedule heterogeneity with regard to certain parameters. Schedule-specific dose–response relationships can then be estimated using shrinkage estimation. Considering Emax models, the proposed method displayed desirable performance in terms of the mean absolute error and the coverage probabilities for the dose–response curve compared to the complete pooling. Furthermore, it outperformed the partial pooling with schedule-specific fixed-effects by producing lower mean absolute error and shorter credible intervals. The methods are illustrated using simulations and a phase II trial example in atopic dermatitis. A publicly available R package, ModStan, is developed to automate the implementation of the proposed method (https://github.com/gunhanb/ModStan).


# Summary. An optional shortened abstract.
summary: We propose a Bayesian hierarchical model with random-effects to model the between-schedule heterogeneity with regard to certain parameters for the phase II trials with multiple schedules. 

tags: [Phase II trials, Bayesian]

# Display this page in the Featured widget?
featured: false 

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2005.04261'
url_code: 'https://github.com/gunhanb/ModStan'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false
---



