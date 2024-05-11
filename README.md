# Data-Scientist-Salary

## Project Overview
This GitHub repository presents a project inspired by Ken Jee, implementing a web scraper originally developed by Omer Sakarya for extracting job listings for Data Scientists from Glassdoor. This initiative aims to delve into the Data Science job market through a comprehensive analysis of job postings. Key stages of the project include utilizing Omer Sakarya's scraping method ((https://mersakarya.medium.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905), cleaning the acquired data to ensure its quality, conducting exploratory data analysis (EDA) to identify significant trends and patterns, and constructing a predictive model to discern the dynamics influencing job opportunities.

## Technologies and Libraries
This project is implemented using Python, leveraging several libraries to manage the data scraping, cleaning, analysis, and modeling phases:

- **Selenium:** Used for automating the web browser to scrape job listings from Glassdoor.
- **Pandas:** Employed for data manipulation and cleaning.
- **NumPy:** Utilized for numerical data handling.
- **Matplotlib and Seaborn:** Used for creating visualizations during the exploratory data analysis.
- **Scikit-learn:** Applied for building and evaluating the predictive model.
These tools were chosen for their robustness and flexibility, allowing for efficient processing and detailed analysis of the job market data.

## Data Preparation
The data preparation process is crucial to ensure the reliability and validity of the analysis. This process includes several key steps:

**Data Scraping:** Using Selenium, job listings are scraped from Glassdoor, following the method established by Omer Sakarya.
**Data Cleaning:** Once the data is collected, it undergoes a rigorous cleaning process to remove inconsistencies or irrelevant information. Specific tasks include:
- Removing duplicate entries.
- Creating new columns
- Converting all salary data to a consistent format.
- Converting all NaN values to -1 to standardize missing data handling.
- Normalizing job titles and company names.
- Standardizing company revenue figures into a uniform format.
**Data Transformation:** Necessary transformations are applied to prepare the dataset for analysis. This involves encoding categorical variables and normalizing numerical data to ensure consistency across the dataset.

## Exploratory Data Analysis (EDA)
The exploratory data analysis (EDA) stage is designed to uncover underlying patterns, relationships, and insights from the cleaned and transformed data. Key aspects of this phase include:

- **Visualization:** Utilizing tools like Matplotlib and Seaborn to create visual representations of the data. Common visualizations include histograms, scatter plots, and box plots to examine the distribution and relationships between variables. Additionally, the WordCloud library is used to visualize text data, highlighting the most frequent terms in job descriptions.
- **Text Analysis:** Leveraging the Natural Language Toolkit (NLTK) for text processing to analyze job descriptions and requirements. This involves tokenizing text, removing stopwords, and other natural language processing techniques to extract meaningful patterns.
- **Statistical Analysis:** Performing statistical tests and calculations to understand the data’s properties. This includes measures of central tendency, dispersion, and correlation tests.
- **Feature Importance:** Identifying which features most significantly affect the target variable, aiding in model selection and refinement.
  
The insights gained from this phase help guide the subsequent modeling process, ensuring that decisions are data-driven and informed.

## Modeling
After thorough exploratory analysis, the modeling phase focuses on building predictive models to interpret the data effectively. This section details the approach and tools used:

- **Model Selection:** Various machine learning models are considered based on the insights and feature importance identified during the EDA. The final choice often depends on the model's performance in terms of accuracy and interpretability.
- **Model Training:** The selected models are trained using the cleaned and processed dataset, ensuring they are well-suited to predict outcomes based on new data.
- **Model Evaluation:** Each model is rigorously evaluated to determine its effectiveness. Metrics such as accuracy, precision, recall, and F1-score are used to assess performance.
- **Model Tuning:** Hyperparameter tuning is conducted to optimize the models for the best possible performance.
This structured approach to modeling ensures that the project outputs are robust and reliable, ready to provide actionable insights.

## Results and Conclusions
This project has successfully developed a model that predicts job market trends for Data Scientists based on data scraped from Glassdoor. The key findings and conclusions are as follows:

- **Trends:** The analysis has revealed significant trends in the job market, such as preferred qualifications, common job titles, and salary ranges.
- **Model Performance:** The predictive model has demonstrated high accuracy and reliability in forecasting job market salarys. Details on model performance metrics (accuracy, precision, recall, F1-score) are provided to substantiate these claims.
- **Insights:** The project provides actionable insights that can help job seekers and employers in the Data Science field to better understand the market and what to provide for it.
- **Future Work:** Potential future enhancements include expanding the dataset to include more geographic locations and incorporating additional variables (i.E. Work Conditions) that may influence job market trends.
