# IBM Data Science Capstone Project

## Overview
This project is part of the **IBM Applied Data Science Capstone** and focuses on analyzing and predicting the successful landing of the **SpaceX Falcon 9 first stage** using data science and machine learning techniques.

SpaceX advertises Falcon 9 launches at a significantly lower cost compared to other providers, largely due to the reusability of the first stage. By predicting whether the first stage will successfully land, we can better estimate launch costs and gain insights into factors that influence mission success.

---

## Objectives
The main objectives of this project are:
- Collect and clean SpaceX launch data from multiple sources
- Perform exploratory data analysis (EDA) to identify key patterns
- Visualize launch sites and outcomes using interactive maps
- Build an interactive dashboard for visual analytics
- Train and evaluate classification models to predict landing success

---

## Project Workflow

### 1. Data Collection and Wrangling
- Collected SpaceX launch data using the SpaceX REST API
- Performed data cleaning, handling missing values and formatting variables
- Converted categorical outcomes into numerical labels for modeling

### 2. Web Scraping
- Scraped Falcon 9 launch records from Wikipedia using **BeautifulSoup**
- Parsed HTML tables and converted them into Pandas DataFrames

### 3. Exploratory Data Analysis (EDA)
- Conducted EDA using **Pandas, Matplotlib, and Seaborn**
- Analyzed relationships between payload mass, orbit type, launch site, and success rate

### 4. SQL Analysis
- Loaded launch data into a database
- Used SQL queries to answer analytical questions related to payload mass, customers, and launch outcomes

### 5. Interactive Visual Analytics with Folium
- Created interactive maps showing:
  - Launch site locations
  - Success and failure outcomes
  - Proximity to coastlines, highways, railways, and cities
- Calculated distances between launch sites and nearby infrastructure

### 6. Dashboard Development with Plotly Dash
- Built an interactive dashboard to visualize:
  - Total successful launches by site (pie chart)
  - Payload mass vs. launch outcome (scatter plot)
- Implemented dropdowns and range sliders for dynamic filtering

### 7. Predictive Analysis (Classification)
- Built and evaluated multiple classification models:
  - Logistic Regression
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)
  - Decision Tree
- Tuned hyperparameters using GridSearchCV
- Evaluated model performance using accuracy and confusion matrices

---

## Results
- **Decision Tree Classifier** achieved the highest accuracy: **94.44%**
- Logistic Regression, SVM, and KNN achieved accuracies around **83.33%**
- Confusion matrix analysis showed no false negatives for the best model, indicating strong reliability in predicting successful landings

---

## Key Insights
- The **CCAFS LC-40** launch site showed the highest overall success rate
- Booster version **FT** demonstrated strong performance across multiple payload ranges
- Payload mass alone does not strongly determine launch success; launch site and booster version play a more significant role

---

## Conclusion
This project demonstrates how data science and machine learning can be applied to real-world aerospace problems. By combining data collection, visualization, interactive dashboards, and predictive modeling, we successfully identified key factors influencing Falcon 9 landing success. The results can support cost estimation and strategic decision-making in competitive space launch markets.

---

## Acknowledgments
- **IBM** for providing the Applied Data Science Professional Certificate
- **Coursera** for hosting the course and learning platform
- **SpaceX** for making launch data publicly available
