# Applying Machine Learning to New Psychoactive Substances Screening

## The Project
The goal of this project is to train and test various machine learning models on the task of screening new psychoactive substances.

The project was inspired by the paper _Screening unknown novel psychoactive substances using GC–MS based machine learning_ (Wong et al., 2023) [[2]](#2).
In the article, the reseachers employ an ANN, a CNN and a Balanced Random Forest to classify various substances. 

This project extends their work by testing more and different ML models and analysing the feature importances.

## New Psychoactive Substances and Machine Learning
According to UNODC, New Psychoactive Substances (NPS) are *substances of abuse, either in a pure form or a preparation, that are not controlled by the 1961 Single Convention on Narcotic Drugs or the 1971 Convention on Psychotropic Substances, but which may pose a public health threat* [source](https://www.sciencedirect.com/science/article/pii/S2468170923000358).
These compounds present a significant challenge since their potential adverse health effects and social harms are often not documented.

Moreover, *the analysis and identification of a large number of chemically diverse substances present in drug markets at the same time is demanding* [[1]](#1).
Therefore, extensive efforts have been made to develop robust and efficient methods for the detection of NPS.

## Credits
Credit is given to the authors of the paper above for inspiring the project and providing the data that is used for training the models. This dataset can be found under the paper's _Appendix D. Supplementary data_. 

## Bibliography
<a name="1"></a>[1] United Nations on Drugs and Crime (UNODC) - Early Warning Advisory on New Psychoactive Substances. https://www.unodc.org/LSS/Page/NPS

<a name="2"></a>[2] Wong, S. L., Ng, L. T., Tan, J., & Pan, J. (2023). Screening unknown novel psychoactive substances using GC–MS based machine learning. *Forensic Chemistry*, 34, 100499. https://www.sciencedirect.com/science/article/pii/S2468170923000358
