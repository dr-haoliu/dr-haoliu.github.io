---
layout: page
title: OPTEC (OPTimal Eligibility Criteria) 
description: A Data-Driven Approach to Optimizing Clinical Study Eligibility Criteria
img: assets/img/project_8/Graphical_Abstract.jpg
importance: 4
category: work
---

## Problem 
Participant recruitment is one of the major barriers to successful human clinical studies. It often suffers from the lack of adequate participants or lack of cohort diversity. Hence, clinical study eligibility design is crucial. Overly restrictive eligibility criteria may lead to delayed or failed recruitment, while unnecessarily broad eligibility criteria may result in the heterogeneity of the study population and impose safety threats on certain population subgroups. 

## What is Already Known
Existing cohort development and validation methods can characterize cohorts meeting given eligibility criteria. However, none of them recommends the most feasible, safe, and diverse eligibility criteria, so users still have to rely on an explorative, trial-and-error process for cohort definition.

## What This Paper Adds 
This work contributes a model called OPTEC (OPTimal Eligibility Criteria) that automatically identifies the optimal clinical study eligibility criteria for a given medical condition with the best tradeoff among feasibility, patient safety, and cohort diversity. We showed that our model could effectively and efficiently optimize eligibility criteria according to user-specified prioritization preferences and generate recommendations based on the top-ranked criteria combination. We also implemented a criteria recommendation system based on OPTEC. It was helpful in recommending feasible candidate eligibility criteria sets and providing actionable knowledge to guide clinical study designers to construct a feasible, safe, and diverse cohort definition during early study design.

 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_8/Graphical_Abstract.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of the criteria combination optimization model (OPTEC). 
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_8/figure1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    2-iteration demonstration of the criteria recommendation system. This figure depicts the interaction between a user and the system.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_8/figure2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Clinical study designer’s interaction with the criteria recommendation system.
</div>

OPTEC model allows flexible attribute configuration and weight settings and an adjustable number of criteria for recommendation and new criteria in the recommended combination per time. It provides flexibility in attribute configurations and applicability in any medical condition or criteria.



