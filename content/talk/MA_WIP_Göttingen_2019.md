+++
date = 2017-01-01T00:00:00  # Schedule page publish date.

title = "Meta-analysis of few studies involving rare events"
time_start = 2019-02-28T16:30:00
time_end = 2019-02-28T17:00:00
abstract = "Meta-analyses of clinical trials targeting rare events face particular challenges when the data lack adequate numbers of events for all treatment arms. Especially when the number of studies is low, standard meta-analysis methods can lead to serious distortions because of such data sparsity. To overcome this, we suggest the use of weakly informative priors (WIP) for the treatment effect parameter of a Bayesian meta-analysis model, which may also be seen as a form of penalization. As a data model, we use a binomial-normal hierarchical model (BNHM) which does not require continuity corrections in case of zero counts in one or both arms. We suggest a normal prior for the log odds ratio with mean 0 and standard deviation 2.82, which is motivated (1) as a symmetric prior centred around unity and constraining the odds ratio to within a range from 1/250 to 250 with 95% probability, and (2) as consistent with empirically observed effect estimates from a set of 37 773 meta-analyses from the Cochrane Database of Systematic Reviews. In a simulation study with rare events and few studies, our BNHM with a WIP outperformed a Bayesian method without a WIP and a maximum likelihood estimator in terms of smaller bias and shorter interval estimates with similar coverage. Furthermore, the methods are illustrated by a systematic review in immunosuppression of rare safety events following paediatric transplantation. A publicly available R package, MetaStan, is developed to automate the Stan implementation of meta-analysis models using WIPs."
abstract_short = ""
event = "Oral presentation at Symposium on meta-analysis of rare events"
event_url = "http://www.ams.med.uni-goettingen.de/download/symposium-2019-02-28.pdf"
location = "Göttingen, Germany"

# Is this a selected talk? (true/false)
selected = true

# Projects (optional).
#   Associate this talk with one or more of your projects.
#   Simply enter the filename of your project file in `content/project/`.
#   Otherwise, set `projects = []`.

# Links (optional).

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

