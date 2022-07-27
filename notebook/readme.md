# Cardio Catch Diseases
## Predicting cardiovascular diseases

## 1. Business Problem.
Cardio Catch Diseases is a company specialized in detecting heart disease in the early stages. Its business model lies in offering an early diagnosis of cardiovascular disease for a certain price.
Currently, the diagnosis of cardiovascular disease is manually made by a team of specialists. The current accuracy of the diagnosis varies between 55% and 65%, due to the complexity of the diagnosis and also the fatigue of the team who take turns to minimize the risks. The cost of each diagnosis, including the devices and the payroll of the analysts, is around $1,000.00.
The price of the diagnosis, paid by the client, varies according to the precision achieved by the team of specialists.

| Exam Accuracy | Price          | Rules                                    | Example                         |
|:--------------|:---------------|:-----------------------------------------|:--------------------------------|
| Above 50%     | min \$500\.00  | \+\$500 for each additional 5% precision | Precision = 55% \-> \$1,000\.00 |
| Up to 50%     | $0\.00         | N/A                                      | N/A                             |

Thus, we see that different values in the exam precision, given by the team of specialists, make the company either have a profitable operation, revenue greater than the cost, or an operation with a loss, revenue less than the cost. This instability of the diagnosis makes the company to have an unpredictable cashflow.
## 2. Business Assumptions.
The assumptions about the business problem is as follows:

- **CVDs are the number 1 cause of death globally**: more people die annually from CVDs than from any other cause.
- An estimated **17.9 million** people died from CVDs in 2016, representing 31% of all global deaths. Of these deaths, 85% are due to heart attack and stroke.
- Over three quarters of CVD deaths take place in **low- and middle-income countries**.
- Out of the **17 million** premature deaths (under the age of 70) due to noncommunicable diseases in 2015, **82%** are in low- and middle-income countries, and 37% are caused by CVDs.
- Most cardiovascular diseases can be **prevented by addressing behavioural risk factors** such as tobacco use, unhealthy diet and obesity, physical inactivity and harmful use of alcohol using population-wide strategies.
- People with cardiovascular disease or who are at high cardiovascular risk (due to the presence of one or more risk factors such as hypertension, diabetes, hyperlipidaemia or already established disease) **need early detection and management** using counselling and medicines, as appropriate.

## 3. Solution Strategy


My strategy to solve this challenge was:

**Step 01. Data Description:** My goal is to use statistics metrics to identify data outside the scope of business.

**Step 02. Feature Engineering:** Derive new attributes based on the original variables to better describe the phenomenon that will be modeled.

**Step 03. Data Filtering:** Filter rows and select columns that do not contain information for modeling or that do not match the scope of the business.

**Step 04. Exploratory Data Analysis:** Explore the data to find insights and better understand the impact of variables on model learning.

**Step 05. Data Preparation:** Prepare the data so that the Machine Learning models can learn the specific behavior.

**Step 06. Feature Selection:** Selection of the most significant attributes for training the model.

**Step 07. Machine Learning Modelling:** Machine Learning model training

**Step 08. Hyperparameter Fine Tunning:** Choose the best values for each of the parameters of the model selected from the previous step.

**Step 09. Convert Model Performance to Business Values:** Convert the performance of the Machine Learning model into a business result.

**Step 10. Deploy Modelo to Production:** Publish the model in a cloud environment so that other people or services can use the results to improve the business decision.
## 4. Top 3 Data Insights

- **false.** People who smoke have more cardiovascular diseases.
- **true.** People up to 30 years old have the least cardiovascular diseases.
- **false.** People who do not practice physical activity have more cardiovascular diseases.
## 5. Machine Learning Model Applied
Tests were made using different algorithms.
## 6. Machine Learning Modelo Performance
The chosen algorithm was the **CatBoost Classifier**. In addition, I made a performance calibration on it.
#### Precision, Recall and other metrics

These are the metrics obtained from the test set.

| precision | recall  | f1\-score | accuracy |
|-----------|---------|-----------|----------|
| 0\.7350   | 0\.7313 | 0\.7331   | 0\.7303  |
## 7. Conclusions
There is still more work to do.
## 8. Lessons Learned
- I learned to convert model to business.

- learned a new algorithm (CatBoost).

- I learned to use confusion matrix
## 9. Next Steps to Improve
- Try to improve Feature Engineering, creating more variables

- Improve my Exploratory Data Analysis with more hypotheses and a mind map.

- Improve my Data Preparation and use better encodings

- Do Hyperparameter Fine Tunning to get better accuracy to increase business value.

- Deploy Model to Production