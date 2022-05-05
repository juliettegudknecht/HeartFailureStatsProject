# Computational Statistics Project - Heart Failure Dataset

# Introduction 
This data set was taken from the UCI repository. It contains the medical records of 299 patients who were diagnosed with heart failure. The data was collected during a follow-up period where each patient had 13 clinical features examined. The data was collected by Davide Chicco and Guiseppe Jurman in 2020 for their research paper “Machine learning can predict survival of patients with heart failure from serum creatinine and ejection fraction alone”.

The purpose of this project is to predict which features are more statistically significant in regards to death event. We intend to focus on model selection and other different statistical prediction methods. Our results will be detailed below.

The limitations to this data set is that it is relatively small which means that even after finding the best model – we would run into problems with under fitting.

# Variable Description 

Thirteen (13) clinical features: - age: age of the patient (years) - anaemia: decrease of red blood cells or hemoglobin (boolean) - high blood pressure: if the patient has hypertension (boolean) - creatinine phosphokinase (CPK): level of the CPK enzyme in the blood (mcg/L) - diabetes: if the patient has diabetes (boolean) - ejection fraction: percentage of blood leaving the heart at each contraction (percentage) - platelets: platelets in the blood (kiloplatelets/mL) - sex: woman or man (binary) - serum creatinine: level of serum creatinine in the blood (mg/dL) - serum sodium: level of serum sodium in the blood (mEq/L) - smoking: if the patient smokes or not (boolean) - time: follow-up period (days) - [target] death event: if the patient deceased during the follow-up period (boolean)

# Conclusion 

After conducting model selection, following conclusions can be made:

The most useful predictor variables, as suggested by AIC criteria, are: age, serum_sodium, sex, ejection_fraction, serum_creatinine, and time.

The overall accuracy rate for logistic regression with given 6 variables is 84%. This accuracy rate is better than the accuracy rate when all the variables are included, i.e, 81.33%

The best predictor models, if all the predictor variables are considered were Linear Disciminant Analysis, and Logistic Regression.

The variables used by tree based method for classification, before pruning, were: ejection_fraction, platelets, serum_creatinine, and time, and after pruning were: ejection_fraction, serum_creatinine, and time.

# Reflection 

Having more observations would have been better. It would have helped us in being more confident about the accuracy rates, and model selection.

Having longer followup period would have made data more reliable.

# Citations

Davide Chicco, Giuseppe Jurman: “Machine learning can predict survival of patients with heart failure from serum creatinine and ejection fraction alone”. BMC Medical Informatics and Decision Making 20, 16 (2020). [Web Link]
