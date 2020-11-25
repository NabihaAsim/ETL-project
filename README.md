# ETL Project Technical Report

The goal of this project was to prepare data using the ETL methodology to understand the impact of the pandemic on the economy in Illinois over the last nine months. The project focused on three sectors of the economy, including small businesses revenue, employment rates and unemployment claims. We began the process by extracting the most valuable data points, transforming the dataset and uploading the data into a SQLdatabase for further analysis. Here was our process: 

# Extract

We received the data from two users on Kaggle in the form of CSV files(https://www.kaggle.com/douglaskgaraujo/opportunity-insights-real-time-economic-tracker-us, https://www.kaggle.com/gpreda/coronavirus-2019ncov ). The economic tracker site had a lot of economic data with different subjects at the state, county and national level. However, we chose small business revenue, employment rate, and unemployment claims at the state level. These subjects were chosen because these were some of the main ways that showed how the economy was affected in each state. 

# Transformation
After we extracted the datafiles, we transformed the data using python and jupyter notebooks. We filtered on one state and dropped columns that were not needed and renamed some columns. Because some columns had object data types, we converted to a numeric data type. To get more concise, readable data, we summarized the data by month. 

# Load

All of the data was uploaded into a relational database using Postgresql. The database contained four main tables: 1) COVID-19 cases; 2) Employment Rate; 3) Unemployment Claims; and 4) Small Business revenue. These tables were chosen so users can compare each category to the number of cases.

# Next Step 
The next step would be to analyze the data to compare the number of COVID-19 cases to the unemployment rates, claims and small business revenue and find correlations, trends, and patterns. 
