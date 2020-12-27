---
title: "Phase I dose-escalation oncology trials with sequential multiple schedules"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Sebastian Weber
- Abdelkader Seroutou
- Tim Friede 


# Author notes (optional)


date: "2021-01-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication:  
publication_short: 

abstract: Phase I dose-escalation trials constitute the first step in investigating the safety of potentially promising drugs in humans. Conventional methods for phase I dose-escalation trials are based on a single treatment schedule only. More recently, however, multiple schedules are more frequently investigated in the same trial. Here, we consider sequential phase I trials, where the trial proceeds with a new schedule (e.g. daily or weekly dosing) once the dose escalation with another schedule has been completed. The aim is to utilize the information from both the completed and the ongoing dose-escalation trial to inform decisions on the dose level for the next dose cohort. For this purpose, we adapted the time-to-event pharmacokinetics (TITE-PK) model, which were originally developed for simultaneous investigation of multiple schedules. TITE-PK integrates information from multiple schedules using a pharmacokinetics (PK) model. In a simulation study, the developed {\color{red}approach} is compared to the bridging continual reassessment method and the Bayesian logistic regression model using a meta-analytic-prior. TITE-PK results in better performance than comparators in terms of recommending acceptable dose and avoiding overly toxic doses for sequential phase I trials in most of the scenarios considered. Furthermore, better performance of TITE-PK is achieved while requiring similar number of patients in the simulated trials. For the scenarios involving one schedule, TITE-PK displays similar performance with alternatives in terms of acceptable dose recommendations. The \texttt{R} and \texttt{Stan} code for the implementation of an illustrative sequential phase I trial example is publicly available (\href{https://github.com/gunhanb/TITEPK_sequential}{https://github.com/gunhanb/TITEPK\_sequential}). In sequential phase I dose-escalation trials, the use of all relevant information is of great importance. For these trials, the adapted TITE-PK which combines information using PK principles is recommended.




# Summary. An optional shortened abstract.
summary: We developed a method to analysze phase I dose-escalation trials with mutiple schedules.

tags: [Phase I dose-escalation trials, Stan]

# Display this page in the Featured widget?
featured: false 

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/1811.09433'
url_code: 'https://github.com/gunhanb/TITEPK_sequential'
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



