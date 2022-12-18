---
layout: page
title: Ontology-based Categorization of Clinical Studies
description: a method for automated ontology-based categorization of clinical studies by their conditions
img: assets/img/project_1/Graph_Abstract.jpg
importance: 1
category: work
---

- **Objective** The free-text Condition data field in the ClinicalTrials.gov is not amenable to computational processes for retrieving, aggregating and visualizing clinical studies by condition categories. This paper contributes a method for automated ontology-based categorization of clinical studies by their conditions. 

- **Materials and Methods** Our method first maps text entries in ClinicalTrials.gov’s Condition field to standard condition concepts in the OMOP Common Data Model by using SNOMED CT as a reference ontology and using Usagi for concept normalization, followed by hierarchical traversal of the SNOMED ontology for concept expansion, ontology-driven condition categorization, and visualization. We compared the accuracy of this method to that of the MeSH-based method. 

- **Results** We reviewed the 4,506 studies on Vivli.org categorized by our method. Condition terms of 4,501 (99.89%) studies were successfully mapped to SNOMED CT concepts, and with a minimum concept mapping score threshold, 4,428 (98.27%) studies were categorized into 31 predefined categories. When validating with manual categorization results on a random sample of 300 studies, our method achieved an estimated categorization accuracy of 95.7%, while the MeSH-based method had an accuracy of 85.0%. 

- **Conclusion** We showed that categorizing clinical studies using their Condition terms with referencing to SNOMED CT achieved a better accuracy and coverage than using MeSH terms. The proposed ontology-driven condition categorization was useful to create accurate clinical study categorization that enables clinical researchers to aggregate evidence from a large number of clinical studies.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_1/Graph_Abstract.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
Our system is comprised of a user-configured module called Category Design and an automatic study categorization pipeline consisting of three modules: 
<ul>
    <li>(1) an information extraction module for extracting concepts from the free-text Condition field and performing necessary preprocessing; </li> 
    <li>(2) a concept normalization module for automatic generation of standardized concepts using Usagi and OMOP CDM standard vocabularies; </li>
    <li>(3) a categorization module for automatically classifying a study to categories. </li>
</ul>
</div>
 

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_1/Figure3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project_1/Figure4.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <li> On the left, we reported the concept matching scores for normalizing 6,209 condition terms extracted from 4501 studies. Out of 6,209 condition terms, Usagi matched 2,673 conditions (43.05%) with the score of 1.0, which means an almost certain correct concept mapping was found for a given condition; 2,444 conditions (39.36%) with scores between 0.9 and 1.0; 428 (6.89%) with 0.8 to 0.9, and 262 (4.22%) with 0.7 to 0.8, indicating close to 93.53% (=43.05%+39.36%+6.89%+4.22%) concepts were normalized with high probability of correctness. This result is encouraging and provides a solid base to use the normalized concepts for the following high-level categorization. </li> 
    <li> On the right, we show the pie chart of the MeSH-based categorization results and the contingency table compared with our method for the 300 studies. In summary, 19 (out of 300) studies did not have MeSH condition term(s), one of which could not be categorized using our method while the other 18 were categorized (16 correctly categorized and 2 miscategorized). Among the other 281 studies, 43 had Different categorization results compared to our method. </li>
</div>



