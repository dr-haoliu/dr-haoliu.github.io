---
layout: page
title: Can Race-sensitive Biomedical Embeddings Improve Healthcare Predictive Models?
description: an algorithm to weigh in race distribution data of clinical research study samples when training biomedical embeddings and evaluate these embeddings for healthcare predictive tasks.
img: assets/img/project_9/figure2.png
importance: 2
category: work
---


<a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10283113/">Paper URL</a>


# Abstract
This reproducibility study presents an algorithm to weigh in race distribution data of clinical research study samples when training biomedical embeddings. We extracted 12,864 PubMed abstracts published between January 1st, 2000 and January 1st, 2022 and weighed them based on the race distribution data extracted from their corresponding clinical trials registered on ClinicalTrials.gov. We trained Word2vec and BERT embeddings and evaluated their performance on predicting length of hospital stay (LHS) and intensive care unit (ICU) readmission using MIMIC-IV electronic health record data. We observed that models trained using race-sensitive embeddings do not consistently outperform the neutral embeddings ones when used for LHS prediction (with similar Mean Absolute Error 1.975 vs. 2.008) or ICU readmission prediction (with similar accuracy 74.61% vs. 75.17% and the same AUC 0.775), respectively. We conclude that demographic sensitive embeddings do not necessarily significantly improve the accuracy of health predictive models as previously reported in the literature.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_9/figure1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
Training process of race-sensitive and natural baseline embeddings
</div>



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_9/figure2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
(a) Feature engineering and encoding of MIMIC-IV patient records and split to training and testing datasets. (b)Training and test process of predicting length of hospital stay and ICU readmission with MIMIC-IV dataset.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_9/figure3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
Estimators and their parameters in Scikit-learn implementation for Length of Hospital Stay and Intensive Care Unit Readmission predictions.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_9/figure4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
LHS prediction comparison between eight predictive models utilizing neutral, race-sensitive embeddings, or without embeddings. The best performance single model is bolded and underscored. The best averaged performance of eight models for four different embeddings are bolded. MAE: Mean Absolute Error; MSE: Mean Squared Error. Significant P-values are marked with an asterisk. “--” indicates that p-value calculation is not applicable. Mann-Whitney U test is performed on MAE.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_9/figure5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
ICU readmission classification comparison between nine classification models utilizing neutral, race-sensitive embeddings, or without embeddings. The best performance single model is bolded and underscored. The best averaged performance of nine models for four different embeddings are bolded. Acc: Accuracy; AUC: Area under curve. “--” indicates that p-value calculation is not applicable. Mann-Whitney U test is performed on accuracy.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_9/figure6.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
Comparison of two best estimators’ performance for LHS and ICU readmission tasks on Black and White populations. Acc: Accuracy; AUC: Area under curve. MAE: Mean Absolute Error; MSE: Mean Squared Error.
</div>







