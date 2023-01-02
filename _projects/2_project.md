---
layout: page
title: CliVER - Toward Scientific Claim Verification on Clinical Trial Publications
description: a research tool to help clinicians/researchers identify relevant evidence in clinical trial studies and assess whether a clinical trial study provides evidence supporting or refuting a clinical claim
img: assets/img/project_2/Graphical_Abstract.png
importance: 1
category: work
---

A CliVER demo is available at https://cliver.chunhualab.org/.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_2/Graphical_Abstract.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The overview of the CliVER pipeline with four major modules: Document collection, Document retrieval, Sentence Selection, and Label prediction.
</div>

- **Objective** To automate clinical evidence retrieval from PubMed and separate supporting and refuting evidence for scientific claims. 
- **Materials and Methods** CliVER is an automated scientific claim verification system that retrieves PubMed abstracts, selects rationale sentences, and predicts labels (Support, Neutral, or Refute) for a given scientific claim using an ensemble of deep masked language models. We evaluated its accuracy by verifying 19 claims from six disease domains against 189,648 abstracts indexed in PubMed between January 2010 to October 2021. CliVER’s label prediction accuracy was further assessed using 15 COVID-19 therapeutic claims against 106 manually selected COVID-19 abstracts.
- **Results** In system-level effectiveness evaluation, CliVER achieved a precision of 79.0% for abstract retrieval, 67.4% for sentence selection, and 63.2% for label prediction, respectively, validated with expert review by four clinicians. In the additional label prediction evaluation using a manually curated COVID-19 corpus, CliVER achieved an F1 score of 0.92, where the ensemble of label prediction models outperforms each individual model by an absolute increase in F1 score from 3% to 11%. 
- **Conclusion** CliVER is the first end-to-end system that shows early promise to automate scientific claim verification for clinical trial publications. Our future work will continue to combine domain knowledge with deep learning models to further improve the retrieval accuracy and the inference capability of CliVER.


<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_2/figure2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_2/figure1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <li>Left: Comparison of the three label prediction models and their majority voting ensemble results on SciFact’s development dataset and CoVERt, respectively. The precision, recall, F1 score are reported, with the highest score for each metric highlighted in bold.</li>
    <li>Right: Accuracy of CliVER under Open setting across six disease domains: Hypertension (5), COVID-19 (5), Rheumatic diseases (15), Digestive system diseases (25), Kidney diseases (20), Alzheimer's disease (25). Study counts for each domain are shown in parentheses.</li>
</div>



