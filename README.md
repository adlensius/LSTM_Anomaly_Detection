# Risk Events and Risk Behaviour Windows Detection with Univariate LSTM Model
A consulting project with Lloyds Banking Group as part of a dissertation presented for the degree of MSc in Statistics with Data Science.

# Goal
This project aims to develop an unsupervised modelling process/framework to detect risk events and risk behaviour windows in Lloyds Banking Group employees' spending activities.

# Overview
Panel data on 2185 Lloyds
Banking Group employees was collected, which included their spending amounts, departments, dates,
days of the week, and time stamps of activities. Two target flags, an indicator of whether an activity is a
risk event and an indicator of whether an activity comprises a risk behaviour window, were also provided
for model evaluation purposes.

Time-series anomaly detection models that can identify risky behaviours were then constructed. The
framework includes model selection, threshold computation, and post-processing to prune false positives
and address weekend effect. The weekend effect refers to any weekend anomalous spending due to it either
being the first weekend spending or that 29 days or longer have passed following its preceding weekend
spending. Furthermore, to preserve the sequential nature of the data, rolling window analysis with a fixed
window of size 5 was implemented. It is crucial for the model to be able to not only accurately detect
risky behaviours to prevent unwanted loss and ensure stability, but also refrain from raising excessive false
alarms to curb unnecessar ty costs and maintain the user’s trust level in the model. Therefore, the F1
score metric, which captures the balance of both criteria, is employed to measure models’ performances.

# Content
S2591760_Dissertation_Anomaly_Detection.pdf is the full report

All code used to generate results and figures are written in the Python notebook Lloyds_Banking_Group_Notebook.ipynb.

The data used is stored in Lloyds_data.csv.

poster_adlensius_fransiskus_djunaedi.pdf is the academic poster for research presentation





