# Uncertainty explanation of AI models

## Title: Uncertainty explanation of artificial intelligence models by SHAP

## Abstract
The “black box” characteristic of AI models has received widespread attention from scientists. This has promoted the development of explainable artificial intelligence (XAI) methods aimed at explaining AI model decisions, e.g., evaluating the importance of input features for the model output. In addition to XAI, another way to open the “black box” is uncertainty estimation of AI models (e.g., output ranges for regression tasks), which provides users with confidence in model decisions. However, little attention has been paid to the explanation of model uncertainty, e.g., which input features contribute to model uncertainty? This study takes SHapley Additive exPlanations (SHAP) as an example of perturbation-based XAI methods and utilizes it to explain AI model uncertainty by changing the model input to observe the variation of the estimated uncertainty. The experimental results in three cases (i.e., housing price prediction, remote sensing image classification, and electrocardiogram classification) show that SHAP can effectively explain the uncertainty of AI models. Moreover, further analysis reveals that the uncertainty of AI models is affected by the frequency of occurrence of input features in the training data. Specifically, if a certain feature of the sample rarely appears in the training data, it will lead to greater uncertainty. This conclusion aligns with common sense and supports the validity of the uncertainty explanation.

## Statement
The program of uncertainty estimation and explanation is developed by Tianqi Wang, please also see his Github ([Uncertainty](https://github.com/wanglaoban1993/Uncertainty)).

## File description
1. The file "houseprice_SHAP_variance_github.ipynb" is the demo program of the experiments including data processing, uncertainty estimation, uncertainty explanation, and explanation evaluation based on the housing price data.
2. The file "housing_price_data.csv" is the experimental data of this demo from an opensource data ([The Boston Housing Dataset](https://www.cs.toronto.edu/~delve/data/boston/bostonDetail.html)).
3. The file "data_split.pickle" is the index group to divide the data into train, validation, and test datasets.
4. The file "trained_model.pth" is the parameters of a trained model to predict the housing price.
5. The file "global_xai_variance_\[0.71805446\].pickle" is an example of uncertainty explanation results with an expected_value=0.71805446.

## Environment
Python 3.9.23

Important Python packages:\\
numpy 1.25.2\\
pandas 1.4.1\\
seaborn 0.13.2\\
matplotlib 3.5.1\\
pytorch 1.10.0\\
scikit-learn 1.6.1\\
shap 0.43.0\\
eli5 0.16.0\\
xgboost 1.5.0\\
scipy 1.9.3\\

## Cite
Please consider citing our paper if this helps in your work:

Ximeng Cheng, Tianqi Wang, Di Zhu, & Jackie Ma (2026). Uncertainty explanation of artificial intelligence models by SHAP. Knowledge-Based Systems. 115437. [DOI](https://doi.org/10.1016/j.knosys.2026.115437)
