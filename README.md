# SpaceX Falcon 9 First Stage Landing Prediction

## Overview
This repository contains the capstone project for the **IBM Data Science Professional Certificate**, focused on predicting the successful landing of SpaceX Falcon 9 first stages. SpaceX's ability to reuse rockets has significantly reduced launch costs, making this prediction model crucial for understanding cost dynamics and providing competitive insights for other aerospace companies.

## Introduction
In this capstone, we predict if the **Falcon 9 first stage** will land successfully. SpaceX advertises Falcon 9 rocket launches at **$62 million**, while other providers charge upwards of **$165 million**. Much of the cost savings come from SpaceX's ability to **reuse the first stage** of their rockets. By predicting the likelihood of a successful landing, we can estimate the **cost of a launch**. This information can be crucial for companies aiming to **compete with SpaceX**.

In this project, you will assume the role of a **Data Scientist** at a startup aiming to rival SpaceX. You'll follow the **Data Science methodology**:

- [Data Collection](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Data%20Collection%20API.ipynb)
- [Data Wrangling](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Data%20Wrangling.ipynb)
- [Exploratory Data Analysis](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/EDA%20with%20SQL.ipynb)
- [Data Visualization](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/EDA%20with%20Data%20Visualization.ipynb)
- [Model Development](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Machine%20Learning%20Prediction.ipynb)
- [Model Evaluation](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Machine%20Learning%20Prediction.ipynb)
- [Reporting](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Winning%20Space%20Race%20with%20Data%20Science.pdf)

## Business Problem
SpaceX's competitive pricing relies on their ability to reuse the first stage of Falcon 9 rockets. By **accurately predicting** whether the first stage will land successfully, companies can **estimate launch costs** and **strategically bid** against SpaceX for contracts.

## Objective
- **Apply data science and machine learning** to predict the likelihood of Falcon 9's first stage landing successfully.
- Perform **data exploration** to uncover insights into the factors affecting rocket landings.

## Business Metric
We use **Classification Accuracy** to evaluate the performance of our predictive models:

$$Accuracy = \frac{TP + TN}{TP + FP + TN + FN}$$

![Confusion matrix](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Plots/Confusion%20matrix.PNG)

## Project Structure

1. **Data Collection**  
   - **[SpaceX API Collection](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Data%20Collection%20API.ipynb)**: Data was fetched using GET requests from the SpaceX API and processed into pandas DataFrames.  
   - **[Web Scraping](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Data%20Collection%20with%20Web%20Scraping.ipynb)**: Additional data on Falcon 9 launches was collected using BeautifulSoup from Wikipedia.

2. **Data Wrangling**  
   - **[Data Cleaning & Feature Engineering](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Data%20Wrangling.ipynb)**: One-hot encoding was applied to categorical features, and missing values were handled appropriately.

3. **Exploratory Data Analysis (EDA)**  
   - **[EDA with Visualization](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/EDA%20with%20Data%20Visualization.ipynb)**: Visual insights were generated to explore relationships between variables like flight number, payload mass, and orbit types.  
   - **[EDA with SQL](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/EDA%20with%20SQL.ipynb)**: SQL queries were used to extract meaningful insights directly from the dataset.

4. **Interactive Visual Analytics**  
   - **[Folium Maps](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/EDA%20with%20Data%20Visualization.ipynb)**: Interactive maps were created to visualize launch sites and outcomes.  
   - **[Plotly Dash Dashboard](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/app.py)**: An interactive dashboard was developed for deeper analysis of launch data.

5. **Predictive Analysis**  
   - **[Machine Learning Models](https://github.com/mukesh16/Applied_Data_Science_Capstone_SpaceX/blob/main/Machine%20Learning%20Prediction.ipynb)**: Various classification models were trained to predict landing outcomes. Hyperparameter tuning with GridSearchCV improved the model performance, and the **Decision Tree Classifier** achieved the highest accuracy.

## Key Results

- **Launch Sites & Success Rates**: The larger the number of flights at a launch site, the higher the success rate.
- **Orbit Analysis**: Orbits like ES-L1, GEO, HEO, SSO, and VLEO had the highest success rates.
- **Machine Learning Outcome**: The Decision Tree Classifier demonstrated the best performance for predicting landing success.
- **Launch Trends**: Success rates have steadily increased from 2013 to 2020.

## Technologies Used
- **Languages**: Python, SQL
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Plotly, Folium, BeautifulSoup, Scikit-learn
- **Tools**: Jupyter Notebook, PostgreSQL, Dash

## Repository Contents
- `Data Collection API.ipynb`: Collecting data via API.
- `Data Collection with Web Scraping.ipynb`: Scraping additional data from Wikipedia.
- `Data Wrangling.ipynb`: Cleaning and preparing the data.
- `EDA with Data Visualization.ipynb`: Visual exploration of the data.
- `EDA with SQL.ipynb`: SQL-based analysis of data.
- `app.py`: Interactive dashboard using Plotly Dash.
- `Machine Learning Prediction.ipynb`: Building and evaluating machine learning models.

## Deliverables
- **Accurate Predictive Models**: Machine learning algorithms that predict landing outcomes.
- **Business Case Report**: Insights and recommendations for stakeholders to make data-driven decisions.

## Conclusion
This project successfully demonstrates how data science and machine learning techniques can be used to predict the outcomes of rocket landings, providing valuable insights for cost optimization and competitive analysis in the aerospace industry.

---

Feel free to explore the notebooks and contribute to the repository!
