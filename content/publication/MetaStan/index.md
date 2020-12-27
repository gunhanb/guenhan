---
title: "Random-effects meta-analysis of few studies involving rare events"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Christian Röver
- Tim Friede 


# Author notes (optional)


date: "2019-08-01T00:00:00Z"
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

abstract: Meta-analyses of clinical trials targeting rare events face particular challenges when the data lack adequate numbers of events for all treatment arms. Especially when the number of studies is low, standard random-effects meta-analysis methods can lead to serious distortions because of such data sparsity. To overcome this, we suggest the use of weakly informative priors (WIP) for the treatment effect parameter of a Bayesian meta-analysis model, which may also be seen as a form of penalization. As a data model, we use a binomial-normal hierarchical model (BNHM) which does not require continuity corrections in case of zero counts in one or both arms. We suggest a normal prior for the log-odds ratio with mean 0 and standard deviation 2.82, which is motivated (1) as a symmetric prior centred around unity and constraining the odds ratio within a range from 1/250 to 250 with 95\% probability, and (2) as consistent with empirically observed effect estimates from a set of 37\,773 meta-analyses from the Cochrane Database of Systematic Reviews. In a simulation study with rare events and few studies, our BNHM with a WIP outperformed a Bayesian method without a WIP and a maximum likelihood estimator in terms of smaller bias and shorter interval estimates with similar coverage. Furthermore, the methods are illustrated by a systematic review in immunosuppression of rare safety events following paediatric transplantation. 



# Summary. An optional shortened abstract.
summary: We developed a method to for the meta-analysis of few studies involving rare events.

tags: [Meta-analysis, Bayesian]

# Display this page in the Featured widget?
featured: false 

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://doi.org/10.1002/jrsm.1370'
url_code: 'https://github.com/gunhanb/MetaStan'
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



