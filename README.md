This repository contains the reproducible workflow and analysis files from our project on modeling breast cancer recurrence, conducted by Carlos Haring and Shiyi Zhang during the University of Michigan Big Data Summer Institute (BDSI).

Using a breast cancer dataset from Duke [1], we analyzed clinically meaningful subgroups of patients with two complementary goals:

1.	Interpretable model (Shiyi Zhang):
To characterize which demographic, pathological, and treatment-related factors were associated with breast cancer recurrence. This included Kaplan–Meier survival analysis, subgroup‐specific Cox proportional hazards models, and time‐dependent ROC assessment to identify variables with prognostic significance and to understand their effects across different molecular subtypes and treatment pathways.

2.  Predictive modeling (Carlos Haring):
To predict recurrence-free survival in breast cancer patients who received neoadjuvant therapy, we built a random survival forest model. Several variables were dichotomized to address imbalance in the dataset. The models were trained using a 4-fold train–test split, and VIMP was used to remove variables that reduced model performance. After 17 iterations, we selected a final model with the highest concordance index (c-index), which was then used to predict recurrence probabilities. We evaluated the model on three patient profiles representing different breast-cancer receptor subtypes to examine predicted recurrence over time.

The repository includes the original data, the cleaned analytic dataset, preprocessing scripts, interpretable and predictive modeling code, our final project poster, and additional visualizations not included in the poster.




[1]. Saha, A., Harowicz, M.R., Grimm, L.J., Kim, C.E., Ghate, S.V., Walsh, R. and Mazurowski, M.A., 2018. A machine learning approach to radiogenomics of breast cancer: a study of 922 subjects and 529 DCE-MRI features. British journal of cancer, 119(4), pp.508-516
