# IPL Data Analytics Project

## Overview
This project utilizes Azure services including Azure Data Lake, Databricks, PySpark, Azure Data Factory, and Synapse Analytics to process and analyze IPL match data. It handles CSV data sourced from GitHub, processes it with sophisticated data manipulation techniques, and prepares it for in-depth analytics.

## Prerequisites
Before you start, ensure the following:
- **Python 3.7+** is installed on your system
- **Git** is installed on your system

# 1. Clone the Repository
Clone the repository to your local machine:
```bash
git clone https://github.com/FaisalxWattoo/IPL_Data_Analytics-End_To_End_Azure_Data_Eng_Project.git
cd IPL_Data_Analytics-End_To_End_Azure_Data_Eng_Project
```

### 2. Install Dependencies
Install the required Python packages using pip:
```bash
pip install -r requirements.txt
```
 
### 3. Set Up Azure Components
Configure Azure Blob Storage and mount it to Databricks. Set up Azure Data Factory to automate the data flow from GitHub to Azure Blob Storage, and use Azure Synapse Analytics for running SQL queries on the processed data. Ensure all configurations and secrets for OAuth authentication are correctly set:
```bash
# Example command for setting up Azure components (not actual commands)
setup_azure_components --setup-storage --setup-data-factory --setup-synapse
```
### 4. Run Data Processing Tasks
Execute the data processing tasks using the Databricks notebooks provided:
```bash
# Run Spark jobs
spark-submit --py-files packages.zip main.py
```
### 5. Explore Data Output
Review the transformed data stored in the Azure Blob Storage under the 'transformed-data' directory.
 
### 6. Access the Processed Data
Use the processed data for further analysis or visualization in tools like Microsoft Power BI
 
### Project Structure

`main.py`: Main application file for Spark jobs
`configs.py`: Configuration settings for Azure
`requirements.txt`: Dependencies for the project

### Contributing
To contribute to the IPL Data Analytics project:

-Fork the repository
-Create a feature branch (git checkout -b feature-branch)
-Commit your changes (git commit -m 'Add some feature')
-Push to the branch (git push origin feature-branch)
-Create a pull request
 
 