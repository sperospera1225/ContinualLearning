# ContinualLearning
Incremental Event Classification for cyber security
* On-going Study for Master's degree


#
# Reviewer Feedback (Weak Reject)

------------------------ METAREVIEW ------------------------Reviewers identified several significant issues 

w.r.t. motivation, positioning 

w.r.t., state of the art, but also clarity 

w.r.t. both methodology and experiments.

**----------------------- REVIEW 1 ---------------------**

SUBMISSION: 4740

TITLE: Research: Stepwise Model Update for Continual Learning in Streaming Event ClassificationAUTHORS: Min-Seon Kim and Hyuk-Yoon Kwon

----------- Overall evaluation -----------

SCORE: -2 (reject)

----- 

TEXT:This paper examines the trade-off between time and effectiveness when updating classification models over time as an event evolves. The authors propose a framework where only some of the components of a model might be updated at each step, depending on the time cost of doing the update and the amount the model is varying. A range of experiments are summarized, examing the relationship between embedding word coverage and effectiveness, and model effectiveness, but these are very difficult to interpret.In terms of the positives of the work. It is good to see papers tacking some of the challenges of real-time machine learning, rather than focusing on retrospective classification. This is a much more difficult challenge, and has not seen much examination. The authors have provided some motivation for their work in terms of training times, and clearly a significant amount of experiments have been done.**On the other hand, the paper from Section 3.2 onward is very difficult to interpret. It seems that the authors have tried to fit in too much into a short paper, and as such key information and explanations are missing.** Specifically, I can not determine how the null embedding indicator (NEI) is calculated, its unclear why the values of NEI reported in Table 3 are chosen, its not clear what the measure of success is for Section 4.3. Indeed, the evaluation metric for Tables 3 and 6 are not defined. Additionally, its unclear why per-event performances are reported if they are never used, and given the temporal nature of the task I was expecting to see performance-over time graphs. Also, why is the selection strategy static? The amount an event evolves changes over time, typically high at the start and lower later. It is also worth noting that the motivation for the task seems rather weak, given that the times reported for model training are quite small (max 15 mins), why not always just do a full update?

----------- Strengths and reasons to accept ------------ 

Tackles are rarer and challenging task

----------- Weaknesses and limitations ------------ 

Aspects are poorly explained 

- Metrics are not clear 

- Researh questions are not defined

**----------------------- REVIEW 2 ---------------------**

SUBMISSION: 4740

TITLE: Research: Stepwise Model Update for Continual Learning in Streaming Event Classification

AUTHORS: Min-Seon Kim and Hyuk-Yoon Kwon

----------- Overall evaluation -----------

SCORE: -1 (weak reject)

----- 

TEXT:Authors present a model update strategy for continual learning of event classification in a real-time data streaming environment.Novelty: okhowever, this paper doesn’t offer any insights in these domains. Several researchers already conducted their continual learning experiments in online setting.

----------- Strengths and reasons to accept 

-----------Tested on real-world dataset.----------- 

Weaknesses and limitations -----------

Lack of literature survey, some continual learning works have considered online setting:Unsupervised Progressive Learning and the STAM ArchitectureMemory-Efficient Semi-Supervised Continual Learning: The World is its Own Replay BufferUnsupervised Continual Learning in Streaming EnvironmentsHow do you position your way to update the model compared to their experiment?

**----------------------- REVIEW 3 ---------------------**

SUBMISSION: 4740

TITLE: Research: Stepwise Model Update for Continual Learning in Streaming Event Classification

AUTHORS: Min-Seon Kim and Hyuk-Yoon Kwon

----------- Overall evaluation -----------

SCORE: -1 (weak reject)

----- 

TEXT:This paper proposes a stepwise update strategy for continual learning of event classification in the streaming environment. The specific analysis on different component (token, embedding, classifier) on time updating is interesting, the description and motivation on strategy decision, the combination of the decision and three component should be improved to make it more clear. Also, for the experiment, the description of implementation, baseline and dataset construction also not clear to be followed.

----------- Strengths and reasons to accept -----------

1. The idea of event shift and the corresponding update strategy is practical

2. The specific analysis on different component (token, embedding, classifier) on time updating is interesting

----------- Weaknesses and limitations -----------

1. The description and motivation on strategy decision, the combination of the decision and three component is not clear, e.g., how to measure the relationship between event shift and the token/embedding? what's the method you plan to update the embedding?

2. Also, for the experiment, the description of implementation, baseline and dataset construction also not clear to be followed.
