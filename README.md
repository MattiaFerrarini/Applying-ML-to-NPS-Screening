# Applying Machine Learning Algorithms to New Psychoactive Substances Screening

## The Project
The goal of this project is to train and test various machine learning models on the task of screening new psychoactive substances.

The project was inspired by the paper _Screening unknown novel psychoactive substances using GC–MS based machine learning_ (Wong et al., 2023) [[1]](#1).
In the article, the reseachers employ an ANN, a CNN and a Balanced Random Forest to classify various substances. 

This project "extends" their work by testing more and different ML models and analysing their feature importances.

## The problem
### New Psychoactive Substances 
According to UNODC, New Psychoactive Substances (NPS) are *substances of abuse, either in a pure form or a preparation, that are not controlled by the 1961 Single Convention on Narcotic Drugs or the 1971 Convention on Psychotropic Substances, but which may pose a public health threat* [[2]](#2).
These compounds present a significant challenge since their potential adverse health effects and social harms are often not documented.

Moreover, *the analysis and identification of a large number of chemically diverse substances present in drug markets at the same time is demanding* [[2]](#2).
Therefore, extensive efforts have been made to develop robust and efficient methods for the detection of NPS.

### Classical approaches to screening NPS
Due to its ease of operation and ability to distinguish compound mixtures, GC–MS is one of the most widely used techniques for substance identification.
Traditionally, the identification of a compound involves matching its retention time and mass spectrum with known records in a library using similarity algorithms. For accurate detection, this approach requires a comprehensive database. However, in the case of NPS, creating an exhaustive database is challenging due to the constantly increasing structural diversity of the substances. Thus, *current GC–MS database are unable to exhaustively cover the spectrum of all possible NPSs* [[1]](#1).

### The machine learning solution
Newer approaches classify unknown substances using machine learning (ML) models trained on compounds in the available library (dataset). These methods are very effective for two reasons:

1. **Pattern recognition**: machine learning algorithms excel at recognizing patterns and trends within complex datasets;
2. **Generalization**: if trained correctly, ML models can generalize the knowledge learned from the available data to new unseen substances, making them particularly suit to detecting substances with always new structures.

An example of this new approach is [[1]](#1), where the authors developed a machine learning based model that can classify an unknown NPS to its drug class based solely on its GC–MS, with no knowledge of its nominal molecular mass.

## The results

| Model         | Accuracy              |
| --------------|:---------------------:|
|XGBoost | 93.85% |
|Stacking |93.30% |
|Majority Voting | 93.30% |
|Random Forest | 93.30% |
|Extra Trees | 90.50% |
|Decision Tree | 79.89% |
|SVM | 77.65% |
|Logistic Regression | 76.54% |
|Gaussian Naive Bayes | 68.16% |
|Nearest Centroid | 67.04% |


## Credits
Credit is given to the authors of [[1]](#1) for inspiring the project and providing the data that was used for training the models. This dataset can be found under the paper's _Appendix D. Supplementary data_. 

## Bibliography
<a name="1"></a>[1] Wong, S. L., Ng, L. T., Tan, J., & Pan, J. (2023). Screening unknown novel psychoactive substances using GC–MS based machine learning. *Forensic Chemistry*, 34, 100499. https://www.sciencedirect.com/science/article/pii/S2468170923000358

<a name="2"></a>[2] United Nations on Drugs and Crime (UNODC) - Early Warning Advisory on New Psychoactive Substances. https://www.unodc.org/LSS/Page/NPS
