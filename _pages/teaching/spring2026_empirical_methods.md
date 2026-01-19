---
layout: default
title: Spring 2026 — COS 598D — Empirical Research Methods for CS
permalink: /teaching/spring2026_empirical_methods

---

<div><br/></div>

<center><h1>Empirical Research Methods for CS</h1></center>
<center><h3>Spring 2026	 — COS 598D</h3></center>
<div><br/></div>

Establishing causal claims and evaluating systems and models are at the core of
modern Computer Science research. This course provides a rigorous introduction 
to empirical methods, combining foundational theory on causal inference with 
practical applications. Topics include causal diagrams, experimental and 
quasi-experimental designs, regression analysis, and benchmarks. 
Evaluation is based on programming assignments, active class 
participation, and a final paper in which students develop and motivate a 
research project proposal.


<hr>

## Table of Contents
1.  [Basic Information](#1-basic-information)
2.  [Schedule](#2-schedule)
3.  [About the course](#3-about-the-course)
4. [Detailed Schedule](#4-detailed-schedule) 
5. [Acknowledgments](#5-acknowledgments) 

<hr>

## 1. Basic information
- **Email:** [manoel@cs.princeton.edu](mailto:manoel@princeton.edu).
- **Office Hours:** on demand.
- **TA:** Romina Mahinpei ([rmahinpei@princeton.edu](mailto:rmahinpei@princeton.edu)).
- **Hours:** Thu, 1:20 pm --- 4:10 pm
- **Location:** TBD.

## 2. Schedule 

|     **Date**      |                                **What?**                                | **Slides** |    **Comment**    |
|:-----------------:|:-----------------------------------------------------------------------:|:----------:|:-----------------:|
| [Jan 29](#jan-29) |                                  Intro                                  | [(TBD)]()  |                   |
| [Feb 05](#feb-05) |                           Potential Outcomes                            | [(TBD)]()  |                   |
| [Feb 12](#feb-12) |                               Experiments                               | [(TBD)]()  |                   |
| [Feb 19](#feb-19) |                           Thinking with DAGs                            | [(TBD)]()  |                   |
| [Feb 26](#feb-26) |                              Regression #1                              | [(TBD)]()  |      HW1 due      | 
| [Mar 05](#mar-05) |                              Regression #2                              | [(TBD)]()  |                   | 
| [Mar 19](#mar-19) |   Benchmarks ([Olawale Salaudeen](https://www.olawalesalaudeen.com/))   | [(TBD)]()  |      HW2 due      |
| [Mar 26](#mar-26) |      Quasi-experiments ([Pietro Lesci](https://pietrolesci.com/))       | [(TBD)]()  |                   | 
| [Apr 02](#apr-02) |            Causal ML ([Drew Dimmery](https://ddimmery.com/))            | [(TBD)]()  |                   |
| [Apr 09](#apr-09) | Labeling with LLMs ([Kristina Gligorić](https://kristinagligoric.com/)) | [(TBD)]()  |                   | 
| [Apr 16](#apr-16) |                    *No Classes (Manoel goes to CHI)*                    |            |                   | 
| [Apr 23](#apr-23) |                           Final Presentations                           | [(TBD)]()  |      HW3 due      | 


## 3. About the course

This course has three central components: 1) reading activities, 2) (guest) lectures, 3) homeworks and project.

### 3.1. Reading Activities

Most weeks will have an assigned reading. I expect you to read these and come prepared to have an informal discussion on the topic at the end of each class.
There is no assignment associated with the readings --- I just expect you to do it.
Assigned readings when guest speakers come will help familiarize students with the topics that will be covered

### 3.2. (Guest) Lectures

Each week, I will give an expository lecture. In the first few weeks, this will take most of the course time.
After spring break, we will have a series of guest speakers, experts doing cutting-edge, relevant research.
In this case, half our class will be an expository lecture by yours truly, and the other half will be a presentation by the guest speaker. 
Students are expected meaningfully engage with the lectures, and in particular with the guest speakers. 

### 3.3. Homework and Project

There will be two homeworks and a project in the course. The first two homeworks will be jupyter notebooks that you must complete individually.
The third project will be to write a project "proposal," using what you learned in the lectures. This can be done in groups or individually.
You are encouraged to mix this project with some research you are already doing, or are already interested in doing.

#### 3.3.1 Homework 1

- **Description**: In a first homework, we will review concepts associated with the design and the analysis of experiments in a machine learning setting.
- **Release date**: Feb 12, 2026.
- **Due date**: Feb 26, 2026.
- **Deliverables**: A filled Jupyter notebook.

#### 3.3.2 Homework 2

- **Description**: In a second homework, we will provide some nut-and-bolts details about running regressions.
- **Release date**: Feb 26, 2026.
- **Due date**: Mar 19, 2026.
- **Deliverables**: A filled Jupyter notebook.

#### 3.3.3 Project

- **Description:** 
  - The final project is to write a research project proposal for an empirical study, using the tools and concepts from the course.
  - From a paper perspective, think of this as writing the paper up to the Methods section. 
  - You may also obtain and present preliminary results, but results are not required and will not be graded. 
  - This project can be done individually or in groups (up to 3 students). 
  - You are encouraged to use this as an opportunity to advance your own research interests.
- **Project types:** Your proposal must describe one of the following:
  - **Experimental study (preferred when feasible):** 
  Design an intervention or randomized experiment and specify:
  1) treatment/control conditions (and what is randomized)
  2) outcome(s) and measurement strategy 
  3) identification assumptions (why this design yields a causal claim)
  4) power considerations or sample size planning (even if approximate)
  5) analysis plan (estimand and statistical model).
  - **Observational / quasi-experimental study:** Propose a study that estimates a causal effect using observational data, and specify:
  1) research question + causal estimand (what effect are you estimating?)
  2) data source(s) and unit of analysis 
  3) identification strategy (e.g., matching, diff-in-diff)
  4) threats to validity and planned robustness checks 
  5) analysis plan (model + sensitivity checks).
  - **Benchmarking/evaluation project:** Propose a benchmark or evaluation framework for a system/model, and specify:
  1) what is being evaluated, and why existing evaluations are insufficient
  2) dataset/task construction plan (including sampling and labeling)
  3) metric design (and why it measures what you claim it measures)
  4) baselines and ablations
  5) expected failure modes and what conclusions would/wouldn’t be justified.
- **Release date:** Mar 19, 2026  
- **Due date:** Apr 23, 2026
- **Deliverables:**
  - **15-minute in-class presentation** during the final session (Apr 23).  
       Your talk should communicate the motivation, the design/identification strategy, and the analysis plan clearly enough that someone else could implement it.
  - **Final report (project proposal)** as a PDF.  
       - **Length:** ~6 pages (single column) .
       - **Format:** any clear academic style (LaTeX encouraged).
- **Evaluation criteria (what I will grade):**
  - Clarity and concreteness of the design
  - Correct use of course concepts
  - Thoughtfulness about threats/failure modes
  - Quality of the analysis plan
  - Communication quality

### 3.4 Grading

- 30% In-class active participation.
- 35% Homeworks 
- 35% Project:
  - 15% Presentation.
  - 20% Final report.


### 3.5. Expectations

- I expect you to:
    - Attend and actively participate in class.
    - Be respectful and collegial to your classmates and guests.
    Complete readings early and submit responses on time to help discussants.
    Present your work when the time comes and serve as a discussant when necessary.
- **Deadlines.** Deadlines exist to help the class run smoothly. However, if you have any extenuating circumstances, please contact me about whether and how you can receive an extension. You must be proactive in letting me know so that we can plan together and others are not disrupted.
- **A note on diversity and respectful conduct.** This course welcomes all students of all backgrounds. You should expect and demand to be treated by your classmates and myself respectfully. If any incident challenges this commitment to a supportive, diverse, inclusive, and equitable environment, please let me know so the issue can be addressed.
- **Disability, Religious, and family accommodations.** If you have any questions about disability or religious accommodations, please refer to university policies. Feel free also to contact me for any reason.
- **Academic integrity.** We will follow the University’s rules and responsibilities guide.

## 4. Detailed Schedule


### Jan 29

- **Course Intro:** 
First, we will frame the course around why empirical reasoning has become central to modern CS: the field’s shift from theory and system building to observation, experiments, and evaluation in the wild.
Second, we will argue that some things are missing from the *style of empiricism* CS relies on.
Finally, we will talk about class logistics.

### Feb 05

- **Potential Outcomes:** 
We introduce the potential outcomes framework: estimands (ATE, ATT), counterfactual reasoning, and what it means to “identify” a causal effect. We will connect these ideas to evaluation of ML models.
- **Reading**: Wallach et al. "[Position: Evaluating Generative AI Systems Is a Social Science Measurement Challenge](https://arxiv.org/abs/2502.00561)," ICML 2025.
*This piece motivates why evaluation in modern AI systems is often not just about accuracy—it requires careful thinking about constructs, measurement, and causal interpretation.*

### Feb 12

- **Experiments:**
We cover randomized experiments: randomization, compliance, treatment effects, interference, power, and common pitfalls (multiple testing, researcher degrees of freedom).
- **Reading**: Hochlehnert et al. "[A Sober Look at Progress in Language Model Reasoning: Pitfalls and Paths to Reproducibility](https://arxiv.org/pdf/2504.07086)," COLM 2025.
*This paper illustrates how empirical claims can be fragile when evaluation pipelines are underspecified or non-reproducible, reinforcing why experimental discipline (pre-specification, careful measurement, robust reporting) matters in ML research.*

### Feb 19

- **Thinking with DAGs:** We introduce causal DAGs as a language for assumptions: confounding, backdoor paths, colliders, mediation, and what it means to “control for” a variable. The emphasis is on reasoning about identification before doing statistics. 
We also introduce matching and propensity scores as practical ways to construct comparable treatment and control groups.
- **Reading**: [Causal Inference: The Mixtape (Chapter 3).](https://mixtape.scunning.com/03-directed_acyclical_graphs)
*This chapter provides the core toolkit for translating causal questions into graphical assumptions, and it sets up the logic we'll need for regression adjustment and "good vs. bad controls" in the next lectures.*

### Feb 26

- **Regression #1:** 
We introduce linear regression from first principles (least squares) and use it as a tool for estimating average treatment effects. We build intuition for what it means to “control for” variables via partialling-out (Frisch–Waugh–Lovell), and extend the basic model with dummy variables and interactions to capture group differences and heterogeneous effects.
- **Reading**: Cinelli et al. "[A Crash Course in Good and Bad Controls](https://ftp.cs.ucla.edu/pub/stat_ser/r493.pdf)," Journal of Sociological Methods and Research 2024.
*This reading makes the "controls" question precise: which variables you should control for depends on the causal structure. It directly builds on DAGs and helps explain why many regressions silently rely on incorrect assumptions.*

### Mar 05

- **Regression #2:** 
We focus on using regression responsibly in empirical work: heteroskedasticity and robust standard errors, basic model diagnostics, and best practices for reporting and interpreting results. We also introduce fixed effects as a practical way to control for unobserved, time-invariant differences across units and briefly discuss the world beyond linear regression.
- **Reading**: [The Effect (Chapter 13).](https://theeffectbook.net/ch-StatisticalAdjustment.html)
*This chapter connects your earlier causal identification ideas (potential outcomes + DAGs/backdoors) to the practical regression workflows people actually use. It discusses many of the intricacies of using regression in practice.*

### Mar 19

- **Benchmarks:** 
We discuss benchmarks as scientific instruments: dataset construction, metric choice, distribution shift, and why repeated evaluation can create illusory progress.   We’ll connect benchmark design to concepts like measurement validity and generalization.
- **Reading**: Recht et al. "[Do ImageNet Classifiers Generalize to ImageNet?](https://proceedings.mlr.press/v97/recht19a.html)," PMLR, 2019.
*By recreating ImageNet-style test sets, the authors show that performance can shift meaningfully even when the intended task is “the same,” highlighting how benchmark scores can quietly bake in dataset-specific quirks and overstate how well models generalize. At the same time, the paper suggests that benchmark progress is not pure illusion: models that perform better on the original test set generally also perform better on the replicated test sets, even if absolute accuracy drops.*
### Mar 26

- **Quasi-experiments:**  We cover causal inference *without* randomized experiments. We focus on two designs: regression discontinuity (RD), and difference in differences. The focus will be on how to articulate an estimand, justify identification assumptions, and run the core diagnostics that make quasi-experimental claims credible.
- **Reading**: Horta Ribeiro et al. "[Automated Content Moderation Increases Adherence to Community Guidelines](https://dl.acm.org/doi/10.1145/3543507.3583275)," TheWebConf, 2023.
*This paper is a concrete, large-scale example of quasi-experimental thinking “in the wild” in a CS-y setting.*
### Apr 02

- **Causal ML:**   We discuss how modern machine learning can be used inside causal inference pipelines: flexible models can learn nuisance components, while carefully constructed estimators still target a well-defined causal estimand with valid uncertainty. The emphasis is on the “separation of concerns”: ML helps estimation, but identification still comes from assumptions and design.
- **Reading**: [Statistical Inference on Predictive and Causal Effects in Modern Nonlinear Regression Models (Chapter 9)](https://causalml-book.org/).
*This chapter is a principled introduction to double / debiased machine learning (DML): it explains why naively plugging ML predictions into causal estimators can introduce bias, and how Neyman-orthogonal moment equations plus cross-fitting (sample splitting) can deliver approximately unbiased estimates and valid inference even with high-dimensional, nonlinear nuisance models.*

### Apr 09

- **Labelling with LLMs:**  We study LLM-based labeling as a measurement pipeline: when it works, when it fails, and how annotation choices (model, prompting, temperature, aggregation) can systematically shape downstream conclusions. We’ll connect this back to measurement validity and researcher degrees of freedom.
- **Reading**: Baumann et al., "[Large Language Model Hacking: Quantifying the Hidden Risks of Using LLMs for Text Annotation](https://arxiv.org/abs/2509.08825,)" arXiv.
*This paper  argues that seemingly innocuous labeling decisions can flip statistical conclusions (“LLM hacking”), quantifying the risks of false positives/negatives in studies that rely on LLM annotations and motivating stricter validation and robustness practices.*

### Apr 16

- No classes.

### Apr 23

- **Final Presentations**

<hr>