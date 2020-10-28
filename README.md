# Covid 19 Patient Status Prediction
**Problem statement**
<br>When the pandemic occurs, flattening the curve helps us to fight against the virus. It is very important to properally and efficiently distrubte the limited medical resources. If we can fastly and accuratly determine if a patient is in severe status, we can better distribute the medical resources. In this project, I build a fast and accurate model to classify the Covid 19 patients into two classes: the positive class is in high risk, who should go to the hospital to use the equipments; the negative class is in good status, who could stay at home to take medicine and have a good rest.

**Inputs**
1. age: age of the patient
2. age_band: age in the unit of decade
3. background_diseases: disease history of the patient
4. background_diseases_binary: whether the patient has a disease history
5. city: city where the patient is from
6. confirmed_date: date when the patient was confirmed with covid 19
7. country: country where the patient is from
8. date_onset_symptoms: date when the patient showed symptoms
9. deceased_date: date when the patient deceased
10. infected_by: number of people the patient was infected by
11. infection_place: where the patient was infected
12. region: region where the patient is from
13. released_date: date when the patient was released
14. return_date: date when the patient returned from travel
15. severity_illness: status of the patient
16. sex: gender of the patient
17. smoking: whether the patient smokes or not
18. symptoms: symptoms of the patient
19. treatment: treatment to the patient
20. id: number index of the patient
21. return_date_until_date_onset_symptoms: days between return and onset of symptoms
22. date_onset_symptoms_until_confirmed_date: days between onset of symptoms and confirmation
23. confirmed_date_until_released_date: days between confirmation and released
24. confirmed_date_until_deceased_date: days between confirmation and deceased
25. severity_illness_infectious_person: status of the infectious person

**Target**
<br>severity = 1 (severity_illness is critical or deceased) or 0 (otherwise)

**Machine learning**
<br>1, Predict severity of a patient based on given informations by applying different models
<br>2, Choose the best model and find out the important features closely related to severity

**Metrics**
<br>Model performance can be evaluated in different ways, here roc_auc is used for classification
<br>ROC_AUC: an ROC curve (receiver operating characteristic curve) is a graph showing the performance of a classification model at all classification thresholds. It plots TPR vs. FPR at different classification thresholds. Lowering the classification threshold classifies more items as positive, thus increasing both False Positives and True Positives. AUC stands for "Area under the ROC Curve." That is, ROC_AUC measures the entire two-dimensional area underneath the entire ROC curve (think integral calculus) from (0,0) to (1,1).
