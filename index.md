---
title: "Data analysis for Cardiovascular Event Predictor"
author: "Agustina Abalo, Tomás Bruno, Tomás Berretta"
date: "14/5/2020"
site: bookdown::bookdown_site
output:
  
   rmdformats::readthedown:
    highlight: espresso # Resalto de sintaxis
    keep_md: yes # Compilar a formato .md
    number_sections: no # Que las secciones/subsecciones tengan número
    self_contained: true # Usar dependencias almacenadas localmente 
    lightbox : yes
    css: style.css
    
---




# Introduction

The data collected to make this graphs was taken from an already curated data set in which there are 1002 patients, from whom: 

- 407 are female
- 595 are male

- Female mean age 47
- Male mean age 50

- 121 suffered a cardiovascular event

This data obtained is representative for this sample but may not apply for all the population.

## Interesting data values:  {.tabset .tabset-fade}

### Mean age of patients who suffered an event {- .unnumbered}

**62.41 years**

### With ongoing pain who had symptoms, older than 62 and suffered an event {- .unnumbered}

**37.04 %**

## Patients according to gender

![](_main_files/figure-html/graphchunk1-1.png)<!-- -->

Women with clinically manifest CHD are in general older than men, with a higher expression of cardiovascular risk factors. Although women and men share most classic risk factors, the significance and the relative weighting of these factors are different. At younger ages (<50 years) smoking is more deleterious in women than in men, with a larger negative impact of the total number of cigarettes smoked per day. Smoking increases the risk of a first acute myocardial infarction (AMI) relatively more in females than in men. In young premenopausal women smoking causes a downregulation of the oestrogen-dependent vasodilatation of the endothelial wall. Whether smoking reduces age at menopause remains a matter of debate.

##  Patients that suffered an event according to risk factors

There are many risk factors for CHD and some can be controlled but not others. The risk factors that can be controlled (modifiable) are: High BP; high blood cholesterol levels; smoking; diabetes; overweight or obesity; lack of physical activity; unhealthy diet and stress. Those that cannot be controlled (conventional) are: Age (simply getting older increases risk); sex (men are generally at greater risk of coronary artery disease); family history; and race.

<!--html_preserve--><div id="htmlwidget-f157272b7a4df60a0a6c" style="width:768px;height:480px;" class="plotly html-widget"></div>
<script type="application/json" data-for="htmlwidget-f157272b7a4df60a0a6c">{"x":{"visdat":{"2d848ba60a5":["function () ","plotlyVisDat"]},"cur_data":"2d848ba60a5","attrs":{"2d848ba60a5":{"y":[13,56,70,75,32,55,45],"x":["Family background","Smoking","Alteration in lipid levels","Hypertension","Diabetes","Obesity","SmeA"],"marker":{"color":["#FFB864","#FFA943","#FF9619","#FA7900","#E77000","#F98C00","#FFC673"]},"alpha_stroke":1,"sizes":[10,100],"spans":[1,20],"type":"bar"}},"layout":{"margin":{"b":40,"l":60,"t":25,"r":10},"xaxis":{"domain":[0,1],"automargin":true,"title":[],"type":"category","categoryorder":"array","categoryarray":["Alteration in lipid levels","Diabetes","Family background","Hypertension","Obesity","SmeA","Smoking"]},"yaxis":{"domain":[0,1],"automargin":true,"title":[]},"hovermode":"closest","showlegend":false},"source":"A","config":{"showSendToCloud":false},"data":[{"y":[13,56,70,75,32,55,45],"x":["Family background","Smoking","Alteration in lipid levels","Hypertension","Diabetes","Obesity","SmeA"],"marker":{"color":["#FFB864","#FFA943","#FF9619","#FA7900","#E77000","#F98C00","#FFC673"],"line":{"color":"rgba(31,119,180,1)"}},"type":"bar","error_y":{"color":"rgba(31,119,180,1)"},"error_x":{"color":"rgba(31,119,180,1)"},"xaxis":"x","yaxis":"y","frame":null}],"highlight":{"on":"plotly_click","persistent":false,"dynamic":false,"selectize":false,"opacityDim":0.2,"selected":{"opacity":1},"debounce":0},"shinyEvents":["plotly_hover","plotly_click","plotly_selected","plotly_relayout","plotly_brushed","plotly_brushing","plotly_clickannotation","plotly_doubleclick","plotly_deselect","plotly_afterplot","plotly_sunburstclick"],"base_url":"https://plot.ly"},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->

Taking into account that patients may suffer from more than one risk factor.


# Analysis 

## Obesity and diabetes


Within this escalating healthcare problem of monumental proportions, obesity-associated type 2 diabetes accounts for 90–95% of all diagnosed diabetes in adults. In fact, diabetes and insulin resistance are powerful predictors of cardiovascular morbidity and mortality, and each is an independent risk factor for death in patients with heart failure. Yet, the complex mechanisms underlying the deleterious impact of diabetes on the heart and vasculature are poorly characterized.

Diabetes-associated cardiovascular diseases arise by a variety of mechanisms. Atherosclerotic disease often emerges in multiple vascular beds. Also, patients with diabetes are often hypertensive. Obesity is associated with a pro-inflammatory state marked by chronic elevations of systemic adrenergic activity, dyslipidemia and hyperglycemia. Circulating levels of a variety of bioactive molecules are perturbed. Clearly, the underlying pathophysiology is complex.

![](_main_files/figure-html/graphAnalysisChunk1-1.png)<!-- -->![](_main_files/figure-html/graphAnalysisChunk1-2.png)<!-- -->

Percentages of patients that suffered an event:

Not Obese and Not Diabetic | Obese and Diabetic | Not Obese and Diabetic | Obese and Not Diabetic
------------ | ------------- | ------------- | -------------
8% | 38% | 14% | 19%

From this graph we can retrieve that patients that suffer either obesity or diabetes are high risk patients but when those two factors are combined there is almost 38% chance of suffering a cardiac event, while only being a 19% with obesity and 14% with diabetic patients.


## Ongoing pain and Acute Coronary Syndrome

Chest pain or discomfort is the most common symptom of the Acute Coronary Syndrome. However, the signs and symptoms can vary significantly based on your age, gender, and other medical conditions. If you are a woman, an older adult, or have diabetes, you are more likely to experience signs and symptoms without chest pain or discomfort.

![](_main_files/figure-html/graphAnalysisChunk2-1.png)<!-- -->![](_main_files/figure-html/graphAnalysisChunk2-2.png)<!-- -->

Percentages of patients that suffered an event:

Not Ongoing Pain and Not SmeA | Ongoing Pain and SmeA | Not Ongoing Pain and SmeA | Ongoing Pain and Not SmeA
------------ | ------------- | ------------- | -------------
6% | 20% | 23% | 11%

This graph shows how SmeA and ongoing pain can be awarded as possible risk factor for cardiac events. As we can see from the graph and statistics, from the patients that had events, a 53% showed positive SmeA and 31% had on going pain.


##  Localized pain

![](_main_files/figure-html/graphAnalysisChunk3-1.png)<!-- -->

Percentages of patients that suffered an event:

Pain in one place | Pain in two places | Pain in three places
------------ | ------------- | -------------
11% | 14% | 22% 

The first pie chart shows in a cualitative way the pain locations in patients while the second pie chart shows the pain location in patients that had an event. Below the graphs, the percentages of patients that suffer  an event have been shown in a table for cuantitative information.


# Predictor


##  Model

To select the variables of our model we used different strategies: 

 - We used the conclusions of our study
 - We made a correlation matrix
 - And we used the result of an automatic variable selection process of machine learning (RFE, from the caret package)

The variables selected are:

  - Age
  - Family History
  - Obesity
  - Alteration in lipid levels
  - Acute Coronary Syndrome
  - Ongoing pain

We decided to use a logistic regression model for the development of the predictor.



## Validation

### Cross Validation

The following boxplot was generated with the 30% of the patients who belong to the test set. (30% of the complete data set)

![](_main_files/figure-html/predChunk2-1.png)<!-- -->

### Analysis of false positives and false negatives from the model

With the predictor finished, 300 people were tested and our model correctly predicts 242 cases, 50 were false positives and 8 were false negatives.




| | Predicted "No Event" | Predicted "Event"
------------ | ------------- | -------------
**Real "No Event"** | 223 | 50 
**Real "Event"** | 8 | 19

### AUROC Curve

![](_main_files/figure-html/predChunk4-1.png)<!-- -->

# Contact

- **Abalo Agustina:** agustina.abalo@ing.austral.edu.ar
- **Berretta Tomás:** tomas.berretta@ing.austral.edu.ar
- **Bruno Tomás:** tomas.bruno@ing.austral.edu.ar

<!--chapter:end:index.Rmd-->

