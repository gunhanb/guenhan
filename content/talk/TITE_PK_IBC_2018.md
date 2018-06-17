+++
date = 2017-01-01T00:00:00  # Schedule page publish date.

title = "Guiding Phase I dose-escalation trials with more than one dosing regimen"
time_start = 2018-07-10T14:00:00
time_end = 2018-07-10T15:00:00
abstract = "Many phase I dose-escalation trials are conducted with flexible dosing regimens, for example starting with a daily dosing and then changing to a weekly dosing. However, standard methods like the Bayesian Logistic Regression Model (BLRM) do not directly allow for more than one dosing regimen to be evaluated, and hence ad-hoc approaches such as simply dose re-scaling are utilized. To overcome this, we propose a new statistical model that uses pharmacokinetic (PK) principles to take into account varying dosing regimens in a model-based approach. We propose to use a latent **pseudo-PK**, which uses the preplanned dosing regimen and the half elimination rate from previous analyses to calculate the exposure measure of the drug. The exposure measure is set proportional to the instantaneous hazard of the time-to-first DLT event process, which gives rise to a time-varying Poisson process. A fully-Bayesian approach is utilized via Stan with weakly informative priors. Our proposed model preserves the advantages of the BLRM, such as interpretable parameters to facilitate defining priors and it allows for the application of the escalation with overdose control principle. The operating characteristics of the proposed procedure were assessed in a Monte Carlo simulation study. The simulation results show that the proposed method has desirable operating characteristics across different true dose-toxicity profiles, especially for combining different dosing regimens scenarios. The proposed method is motivated and illustrated by a real-life example."
abstract_short = ""
event = "Poster presentation at IBC conference"
event_url = "http://2018.biometricconference.org"
location = "Barcelona, Spain"

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

