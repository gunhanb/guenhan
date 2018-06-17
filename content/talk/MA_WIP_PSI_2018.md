+++
date = 2017-01-01T00:00:00  # Schedule page publish date.

title = "Meta-analysis of rare events with few studies"
time_start = 2018-06-03T17:00:00
time_end = 2018-06-03T19:00:00
abstract = "Meta-analysis of clinical trials for rare events faces particular challenges when the data lack adequate numbers of events for all treatment arms. Especially when the number of studies is low, standard meta-analysis methods can lead to serious distortions because of such data sparsity; in the extreme, the resulting estimates of treatment effect can take implausibly huge or even infinite values. To overcome this, we suggest the use of *weakly informative priors* (WIP) for the effect parameter of a Bayesian meta-analysis model as a form of penalization. As a data model, we use a generalized linear mixed model (GLMM) which does not require a continuity correction in case of zero counts. We suggest a normal prior with zero mean and standard deviation 2.82, which is motivated as follows. Firstly,  it represents a priori information that the underlying odds ratio is between 1/250 and 250 with 95% probability. Secondly, it is consistent with effect estimates empirically observed in a set of 37 773 meta-analyses from the Cochrane Library with binomial endpoints. The properties of different (Bayesian and frequentist) meta-analysis methods are assessed in a simulation study. Furthermore, the methods are illustrated by a systematic review in immunosuppression of rare safety events following pediatric transplantation. With rare events and few studies, our GLMM model with a WIP outperformed other alternatives in terms of smaller bias and shorter interval estimates with similar coverage. A publicly available **R** package, **MetaStan**, is under development to automate the **Stan** implementation of meta-analysis models using WIP."
abstract_short = ""
event = "Poster presentation at PSI annual conference"
event_url = "https://www.psiweb.org/psi-2018/psi-conference-2018"
location = "Amsterdam, Holland"

# Is this a selected talk? (true/false)
selected = true

# Projects (optional).
#   Associate this talk with one or more of your projects.
#   Simply enter the filename of your project file in `content/project/`.
#   Otherwise, set `projects = []`.
projects = []

# Links (optional).
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

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

