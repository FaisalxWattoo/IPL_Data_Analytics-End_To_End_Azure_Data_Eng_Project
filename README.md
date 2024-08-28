# IPL Data Analytics Project

## Overview
This project leverages Azure Data Lake, Databricks, PySpark, Azure Data Factory, and Synapse Analytics to process and analyze IPL match data. It handles CSV data sourced from GitHub, transforms it using sophisticated data manipulation techniques, and prepares it for in-depth analytics.

## Prerequisites
Before you start, ensure the following tools are installed on your system:
- **Python 3.7+**
- **Git**

# 1. Clone the Repository
Clone the repository to your local machine:
```bash
git clone https://github.com/FaisalxWattoo/IPL_Data_Analytics-End_To_End_Azure_Data_Eng_Project.git
cd IPL_Data_Analytics-End_To_End_Azure_Data_Eng_Project
```
### 2. Create and Activate a Virtual Environment
It's recommended to use a virtual environment to manage dependencies:
 
```bash
# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
 
# On Windows
python -m venv venv
.\venv\Scripts\activate
```
### 3. Install Dependencies
Install the required Python packages using pip:
```bash
pip install -r requirements.txt
```
 
### 4. Set Up Azure Components
Configure Azure Blob Storage and mount it to Databricks. Set up Azure Data Factory to automate the data flow from GitHub to Azure Blob Storage, and use Azure Synapse Analytics for running SQL queries on the processed data. Ensure all configurations and secrets for OAuth authentication are correctly set:
```bash
# Example command for setting up Azure components (not actual commands)
setup_azure_components --setup-storage --setup-data-factory --setup-synapse
```
### 5. Run Data Processing Tasks
Execute the data processing tasks using the Databricks notebooks provided:
```bash
# Run Spark jobs
spark-submit --py-files packages.zip main.py
```
The application will start on http://127.0.0.1:8000.
 
### 6. Explore Data Output
Review the transformed data stored in the Azure Blob Storage under the 'transformed-data' directory.
 
### 7. Access the Processed Data
Use the processed data for further analysis or visualization in tools like Microsoft Power BI
 
### Project Structure

`main.py`: Main application file for Spark jobs
`configs.py`: Configuration settings for Azure
`requirements.txt`: Dependencies for the project
`venv/`: Virtual environment (not included in the repository)

### Contributing
To contribute to the IPL Data Analytics project:

-Fork the repository
-Create a feature branch (git checkout -b feature-branch)
-Commit your changes (git commit -m 'Add some feature')
-Push to the branch (git push origin feature-branch)
-Create a pull request
 
 