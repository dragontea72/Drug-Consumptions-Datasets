
# Enhanced Multi-Drug Use Prediction Using Optimized Classical Machine Learning and Hybrid Voting Ensemble Methods

## Author Information

**Riadul Islam Rabbi**  
Faculty of Engineering and Technology  
Multimedia University (MMU) 
Malaysia  
Email: riadul.rabbi72@gmail.com  

**Ekramul Haque Tusher**  
Faculty of Computing  
University Malaysia Pahang Al-Sultan Abdullah  
Malaysia  
Email: ekramulhaquetusher@gmail.com  

**Fatema Mostafa Tarin**  
Department of Computer Science and Engineering  
International Islamic University Chittagong  
Bangladesh  
Email: f.m.tarin.cse@gmail.com  

**Jia Uddin**  
AI and Big Data Department  
Woosong University  
Daejeon, Republic of Korea  
Email: jia.uddin@wsu.ac.kr  

---
A machine learning framework for **multi-drug use prediction** using optimised classical models and a **hybrid voting ensemble**, designed to improve predictive reliability across multiple substance categories.

---

## Overview

Drug-related classification remains challenging because biomedical and behavioural data are often heterogeneous, high-dimensional, and difficult to model with default machine learning settings. This project presents a structured framework that combines preprocessing, exploratory analysis, hyperparameter tuning, and ensemble learning to improve prediction performance across multiple drug categories. 

The study investigates prediction performance for ten substances:

- Cocaine
- Heroin
- Nicotine
- Alcohol
- Benzodiazepines
- LSD
- Mushrooms
- Ecstasy
- Caffeine
- Cannabis

Six baseline models and one ensemble strategy were explored:

- Logistic Regression
- Support Vector Machine (SVM)
- AdaBoost
- Ridge Classifier / Ridge Regression-based classifier
- Random Forest
- Decision Tree
- Hybrid Hard Voting Ensemble

---

## Key Contributions

- Develops a complete end-to-end framework for **multi-drug use prediction**
- Benchmarks multiple **classical machine learning algorithms**
- Improves baseline performance through **feature engineering** and **hyperparameter tuning**
- Introduces a **hybrid voting ensemble** for improved robustness
- Evaluates model behaviour across **ten different drug categories**
- Supports reproducible experimentation for future public health and drug prediction research

---

## Abstract

This study addresses the limitations of baseline machine learning models in multi-drug use prediction by applying targeted optimisation and ensemble learning. Six classical machine learning algorithms were evaluated across ten substance categories using accuracy, precision, recall, and F1-score. After preprocessing, feature engineering, and hyperparameter tuning, model performance improved substantially. Random Forest consistently delivered the strongest results across most categories, while the hybrid voting ensemble performed especially well on harder-to-classify classes such as Heroin and Caffeine. These findings show that carefully tuned classical methods can provide a practical and scalable approach for robust drug-related classification. 

---

## Methodology

The proposed framework follows a structured pipeline:

1. **Data acquisition**  
   Primary and secondary data containing demographic, behavioural, and drug-related attributes were collected.

2. **Data preprocessing**  
   - Missing value handling  
   - Label encoding for categorical variables  
   - Standardisation of numerical features  

3. **Exploratory Data Analysis (EDA)**  
   Feature distributions, outliers, and correlations were examined.

4. **Train-test split**  
   The dataset was divided into:
   - **80% training**
   - **20% testing**

5. **Model training**  
   Multiple machine learning models were trained for each drug category.

6. **Hyperparameter tuning**  
   Grid Search Cross-Validation was used to optimise model settings.

7. **Evaluation**  
   Performance was assessed using:
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion matrix analysis
   - Statistical testing

This pipeline was designed to improve generalisation while reducing underfitting and overfitting. :contentReference[oaicite:7]{index=7} :contentReference[oaicite:8]{index=8}

---

## Models Used

The following models were included in the study:

- Logistic Regression
- Support Vector Machine (SVM)
- AdaBoost Classifier
- Ridge Classifier
- Decision Tree
- Random Forest
- Hybrid Hard Voting Ensemble

Among these, **Random Forest** consistently achieved the strongest overall performance, while the **hybrid voting ensemble** improved prediction for more difficult substance classes. 

---

## Main Findings

- **Random Forest** showed the best overall results across most drug categories.
- For **Cocaine**, some models achieved **perfect classification performance**.
- **Heroin** and **Nicotine** were more challenging than other substances.
- Hyperparameter tuning significantly improved predictive strength.
- The **hybrid voting ensemble** outperformed individual classifiers on difficult categories such as **Heroin** and **Caffeine**.
- Retraining and optimisation improved confusion matrix outcomes across all ten drug categories.
- 
---

## Statistical Analysis

The study also included statistical analysis to assess:

- The relationship between **age** and **user status**
- The relationship between **model scores** and **drug use**
- Whether observed performance differences were statistically meaningful

The reported ANOVA results supported the significance of model differences for several drug categories, especially for more complex substances such as Heroin, LSD, Mushrooms, and Ecstasy. 

---


# Drug-Consumptions-Datasets
Classify type of drug consumer by personality data
# Drug Consumption Prediction Research Dataset

This repository contains the dataset files used in our research on drug consumption prediction and multi-drug use analysis. The data are derived from the **Drug Consumption (Quantified)** dataset, which is available through the UCI Machine Learning Repository and mirrored on Kaggle. The original dataset includes records for **1,885 respondents**, with demographic, personality, impulsivity, and sensation-seeking attributes, along with drug consumption labels across multiple substances. 


This datasets can be used for:

- multi-class classification for each drug separately,
- binary drug use classification,
- risk prediction of drug consumption,
- behavioural and personality-based drug use analysis.
## Dataset Sources

### Dataset 1: Original Public Dataset
- **Name:** Drug Consumptions (UCI)
- **Source (Kaggle):** [Drug Consumptions (UCI)](https://www.kaggle.com/datasets/obeykhadija/drug-consumptions-uci)
- **Original Repository:** UCI Machine Learning Repository
- **DOI:** `10.24432/C5TC7S` 

### Dataset 2: Research-Prepared Version
This repository also includes a processed or selected version of the dataset used in our experiments:

- **File:** `drug_raw_consumption1.csv`
- **Purpose:** Research-specific subset / cleaned version used for analysis and modelling in this study

## Dataset Description

The original Drug Consumption dataset contains demographic and psychological measurements such as:

- Age
- Gender
- Education
- Country
- Ethnicity
- Neuroticism score (`Nscore`)
- Extraversion score (`Escore`)
- Openness score (`Oscore`)
- Agreeableness score (`AScore`)
- Conscientiousness score (`Cscore`)
- Impulsiveness
- Sensation Seeking

It also includes drug consumption classes for multiple substances. In the original dataset, each drug is labelled using **seven classes**:

- `CL0` = Never Used
- `CL1` = Used over a Decade Ago
- `CL2` = Used in Last Decade
- `CL3` = Used in Last Year
- `CL4` = Used in Last Month
- `CL5` = Used in Last Week
- `CL6` = Used in Last Day :contentReference[oaicite:2]{index=2}

## Files in This Repository

- `drug_raw_consumption1.csv` — dataset version used in our research
- `README.md` — dataset description and source information

## Structure of the Included CSV File

The included research CSV file contains **1,938 rows and 23 columns**, including:

### Input Features
- `ID`
- `Age`
- `Gender`
- `Education`
- `Country`
- `Ethnicity`
- `Nscore`
- `Escore`
- `Oscore`
- `AScore`
- `Cscore`
- `Impulsive`
- `SS`

### Target / Drug-Use Variables
- `Alcohol`
- `Caff`
- `Choc`
- `Coke`
- `Ecstasy`
- `Heroin`
- `LSD`
- `Mushrooms`
- `Nicotine`
- `Benzos`

## Research Use

This dataset was used for research purposes only. The repository is intended to:

- provide transparency for experimental data usage,
- support reproducibility,
- document the original public source,
- and make the research-specific dataset version easy to reference.

## Reference Paper

Fehrman, E., Muhammad, A. K., Mirkes, E. M., Egan, V., and Gorban, A. N.  
**The Five Factor Model of Personality and Evaluation of Drug Consumption Risk**.  
arXiv, 2015.

## Citation

If you use this dataset, please cite the original dataset source and associated publication.

## Acknowledgements

We acknowledge the original dataset creators:

- **Elaine Fehrman**
- **Vincent Egan**
- **Evgeny M. Mirkes**

Their contributions made this dataset publicly available for research purposes.

##License and Credit

The public dataset is distributed under the CC BY 4.0 license through the UCI Machine Learning Repository. Please give appropriate credit to the original creators when using or redistributing the data.

##Acknowledgement

We acknowledge the original creators of the Drug Consumption dataset and the UCI Machine Learning Repository / Kaggle source for making the data publicly accessible.

## How to Use

You can load the included CSV file in Python as follows:

```python
import pandas as pd

df = pd.read_csv("drug_raw_consumption1.csv")
print(df.head())
print(df.shape)
```
@article{rabbi2026multidrug,
  title={Enhanced Multi-Drug Use Prediction Using Optimized Classical Machine Learning and Hybrid Voting Ensemble Methods},
  author={Rabbi Riadul Islam, Tusher Ekramul Haque, Tarin Fatema Mostafa and Uddin Jia},
  journal={ },
  year={2026}
}
