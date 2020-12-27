---
title: "A design‐by‐treatment interaction model for network meta‐analysis and meta‐regression with integrated nested Laplace approximations"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Tim Friede 
- Leonhard Held

# Author notes (optional)


date: "2017-11-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2019-08-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In Research Synthesis Methods
publication_short: In Research Synthesis Methods

abstract: Network meta‐analysis (NMA) is gaining popularity for comparing multiple treatments in a single analysis. Generalized linear mixed models provide a unifying framework for NMA, allow us to analyze datasets with dichotomous, continuous or count endpoints, and take into account multiarm trials, potential heterogeneity between trials and network inconsistency. To perform inference within such NMA models, the use of Bayesian methods is often advocated. The standard inference tool is Markov chain Monte Carlo (MCMC), which is computationally expensive and requires convergence diagnostics. A deterministic approach to do fully Bayesian inference for latent Gaussian models can be achieved by integrated nested Laplace approximations (INLA), which is a fast and accurate alternative to MCMC. We show how NMA models fit in the class of latent Gaussian models and how NMA models are implemented using INLA and demonstrate that the estimates obtained by INLA are in close agreement with the ones obtained by MCMC. Specifically, we emphasize the design‐by‐treatment interaction model with random inconsistency parameters (also known as the Jackson model). Also, we have proposed a network meta‐regression model, which is constructed by incorporating trial‐level covariates to the Jackson model to explain possible sources of heterogeneity and/or inconsistency in the network. A publicly available R package, nmaINLA, is developed to automate the INLA implementation of NMA models, which are considered in this paper. Three applications illustrate the use of INLA for a NMA.



# Summary. An optional shortened abstract.
summary: We developed a method to for the meta-analysis of few studies involving rare events.

tags: [Meta-analysis, Bayesian]

# Display this page in the Featured widget?
featured: false 

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://doi.org/10.1002/jrsm.1285'
url_code: 'https://github.com/gunhanb/nmaINLA'
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



