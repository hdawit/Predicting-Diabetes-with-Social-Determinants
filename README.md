# Predicting-Diabetes-with-Social-Determinants
### Introduction and Project Overview
Diabetes is a prevalent and chronic health condition that affects millions of individuals worldwide. Understanding the factors contributing to the onset of newly diagnosed diabetes cases is crucial for effective prevention and management strategies. This project aims to develop a predictive model that can estimate the rate of newly diagnosed diabetes based on various demographic, socioeconomic, and health-related factors.

The objective of this predictive model is to build a machine learning model that accurately predicts the rate of newly diagnosed diabetes cases in the United States. By analyzing various features such as obesity rate, physical inactivity, population demographics, socioeconomic indicators, and healthcare availability, the model will identify key predictors and risk factors associated with the onset of diabetes.

### Dataset Source and Preprocessing
The dataset used in this project was obtained from the Centers for Disease Control and Prevention (CDC) website (https://gis.cdc.gov/grasp/diabetes/diabetesatlas-sdoh.html). It consists of information at the county level, including variables such as the number of diagnosed diabetes cases, obesity rate, physical inactivity rate, poverty levels, educational attainment, healthcare accessibility, and other social determinants of health. The dataset contains 3149 entries, with 18 columns providing insights into various factors relevant to diabetes.

To prepare the dataset for analysis, several preprocessing steps were performed:

Loading Multiple Datasets: More than 20 datasets were obtained from the CDC website (https://gis.cdc.gov/grasp/diabetes/diabetesatlas-sdoh.html). Each dataset contained information on various socio-demographic and health-related factors associated with diabetes. These datasets were loaded and merged to create a comprehensive dataset for analysis.

Dataset Merging: The individual datasets were merged based on a common identifier, such as CountyFIPS, to combine the relevant information into a single dataset. This allowed for a holistic analysis of the factors influencing newly diagnosed diabetes cases.

Handling Missing Values: The dataset was examined for missing values. Rows with missing values were dropped to ensure the integrity of the data and to prevent any potential biases in the analysis.

Column Renaming and Reordering: The column names were reviewed and modified to enhance clarity and consistency. Additionally, the columns were reordered to improve the logical flow and ease of analysis.

Exploratory Data Analysis (EDA)
Diagnosed Diabetes Cases by State
The following graph displays the variability in diagnosed diabetes cases across different states:

<img width="1171" alt="Screenshot 2023-07-30 at 2 38 22 PM" src="https://github.com/hdawit/Predicting-Diabetes-with-Social-Determinants/assets/43795941/2c3c30d3-33d6-468b-b738-b6835aae0da9">

### Key Observations:

Variability: The diagnosed diabetes cases exhibit significant variability across different states, as evident from the wide range of heights in the box plots. This suggests a notable disparity in the prevalence of diabetes cases among states.

Outliers: Texas stands out with a remarkably high number of diagnosed cases, indicating a potentially higher prevalence or unique factors contributing to diabetes in that state. Conversely, Vermont stands out with a relatively lower number of diagnosed cases, suggesting a potentially lower prevalence or effective preventive measures.

State Comparison: California emerges as a standout state with a high median and a wide interquartile range, indicating a substantial prevalence of diagnosed diabetes cases compared to other states. This observation highlights the need for targeted interventions and healthcare policies to address the diabetes burden in California.

Lowest Prevalence: On the other end of the spectrum, North Dakota and Wyoming display relatively lower diagnosed diabetes cases. Their lower medians and narrower interquartile ranges suggest a comparatively lower prevalence of diabetes in these states. Understanding the factors contributing to this lower prevalence could provide insights into preventive strategies that can be applied in other regions.

### Scatter plot of Diagnosed using Obesity and Physical Inactivity

The following scatter plot visualizes the relationship between diagnosed diabetes cases, obesity rate, and physical inactivity:

<img width="1120" alt="Screenshot 2023-07-30 at 2 43 20 PM" src="https://github.com/hdawit/Predicting-Diabetes-with-Social-Determinants/assets/43795941/dbbb39d8-2a6d-434a-a9de-4ec3a0d38952">

### Key Observations:

Positive Relationship: There seems to be a positive relationship between obesity and physical inactivity. As the obesity level increases, the physical inactivity also tends to increase.

Diagnosed Diabetes Cases: The color of the markers represents the number of diagnosed diabetes cases. The plot shows that higher levels of obesity and physical inactivity are associated with a higher number of diagnosed diabetes cases, indicated by the darker color of the markers.

Concentration: The scatter plot shows that there is a concentration of diagnosed diabetes cases in the higher range of obesity and physical inactivity. This suggests that individuals with higher levels of obesity and physical inactivity are more likely to be diagnosed with diabetes.

Varied Diagnosed Cases: The plot also reveals that there are diagnosed diabetes cases across a range of obesity and physical inactivity levels. It indicates that obesity and physical inactivity alone may not be the sole factors contributing to diabetes, as there are individuals with lower levels of these factors who are also diagnosed with the disease.

### Scatter Plots: Newly Diagnosed Cases vs Various Features
The following scatter plots illustrate the relationships between newly diagnosed diabetes cases and various features:

<img width="1056" alt="Screenshot 2023-07-30 at 2 40 23 PM" src="https://github.com/hdawit/Predicting-Diabetes-with-Social-Determinants/assets/43795941/7291ed3d-0c3b-4264-b1c9-582f38662401">

### Key Observations:

Crowding: Higher crowding levels may be associated with a higher number of newly diagnosed diabetes cases.

Unemployment: Areas with higher unemployment rates tend to have more newly diagnosed diabetes cases.

Severe Housing Cost Burden: There is a potential relationship between severe housing cost burden and newly diagnosed diabetes cases.

Overall Household Composition & Disability: No clear relationship observed between overall household composition & disability and newly diagnosed diabetes cases.

Overall Housing Type & Transportation: No clear relationship observed between overall housing type & transportation and newly diagnosed diabetes cases.

Population Minority: No clear relationship observed between population minority and newly diagnosed diabetes cases.

Population No Health Insurance: Higher population without health insurance is associated with more newly diagnosed diabetes cases.

Population No High School Diploma: Higher population without a high school diploma is associated with more newly diagnosed diabetes cases.

Number of Primary Care Physicians: No clear relationship observed between the number of primary care physicians and newly diagnosed diabetes cases.

### Conclusion
In this predictive modeling project, we aimed to predict the number of "Newly_Diagnosed" diabetes cases using demographic, socioeconomic, and health-related factors. Various regression models were built and compared, with the Gradient Boosting model demonstrating the most promising results. However, despite its performance, there remains potential for improvement. Therefore, we propose exploring deep neural networks to capture more complex relationships in the dataset and further refining the dataset by incorporating genomic data and personalized medicine information.

### Key Findings
While the initial Linear Regression model displayed suboptimal performance, the Random Forest and Gradient Boosting models showed promise, with the Gradient Boosting model outperforming in terms of R2 score.

Advanced ensemble methods, although useful, still left room for improvement in predictive accuracy. This gap highlights the potential benefits of employing more sophisticated modeling techniques, like deep neural networks.

### Future Steps
To further enhance the predictive power of our models, we propose exploring deep learning techniques, specifically deep neural networks. Deep neural networks can capture highly complex, non-linear relationships and interactions in data that traditional machine learning models may miss. They have the potential to significantly improve predictive accuracy and provide a more nuanced understanding of the factors influencing newly diagnosed diabetes cases.

Additionally, we plan to refine the dataset by incorporating genomic data and information related to personalized medicine. Genomic data can offer insights into genetic predispositions to diabetes, thus providing a more comprehensive view of the factors contributing to disease onset. This kind of data could reveal unique patterns and interactions that are not apparent in the current set of variables.

In terms of personalized medicine, incorporating this data can help tailor prevention and management strategies to individual needs. It can provide information about how different individuals might respond to various interventions, thereby allowing for more targeted and effective strategies. Integrating this information into the model could enhance its predictive power and its applicability in real-world scenarios.

In summary, the future focus will be on leveraging deep neural networks and enhancing the dataset with genomic data and personalized medicine information. The ultimate goal remains to understand the factors contributing to new diabetes diagnoses better, which would help formulate more effective, personalized prevention, and management strategies.
