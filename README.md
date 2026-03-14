# Drug-Consumptions-Datasets
Classify type of drug consumer by personality data
# Drug Consumption Prediction Research Dataset

This repository contains the dataset files used in our research on drug consumption prediction and multi-drug use analysis. The data are derived from the **Drug Consumption (Quantified)** dataset, which is available through the UCI Machine Learning Repository and mirrored on Kaggle. The original dataset includes records for **1,885 respondents**, with demographic, personality, impulsivity, and sensation-seeking attributes, along with drug consumption labels across multiple substances. :contentReference[oaicite:0]{index=0}


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
- **DOI:** `10.24432/C5TC7S` :contentReference[oaicite:1]{index=1}

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
