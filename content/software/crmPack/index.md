---
title: crmPack
summary: Object-Oriented Implementation of CRM Designs
tags:
- phase I dose-escalation trials
date: "2022-09-02T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""


links:
- icon: github
  icon_pack: fab
  name: Github page
  url: https://github.com/roche/crmPack
url_code: https://cran.r-project.org/package=crmPack
url_pdf: https://cran.r-project.org/web/packages/crmPack/vignettes/example.pdf
url_slides: ""
url_video: ""


---
I am in the development team of the R package **crmPack**.

**Description**: Implements a wide range of model-based dose escalation designs, ranging from classical and modern continual reassessment methods (CRMs) based on dose-limiting toxicity endpoints to dual-endpoint designs taking into account a biomarker/efficacy outcome. The focus is on Bayesian inference, making it very easy to setup a new design with its own JAGS code. However, it is also possible to implement 3+3 designs for comparison or models with non-Bayesian estimation. The whole package is written in a modular form in the S4 class system, making it very flexible for adaptation to new models, escalation or stopping rules.
