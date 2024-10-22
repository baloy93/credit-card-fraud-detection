# credit-card-fraud-detection

This project implements a data pipeline for Credit Card Fraud Detection using various Azure services. A Jupyter Notebook is used to generate and simulate credit card transaction data, which is processed in real time using Azure Stream Analytics. The processed data is transformed in Azure Databricks and visualized in Power BI to identify fraud patterns.

Key Features;
Data Simulation: A Jupyter Notebook is used to generate synthetic credit card transaction data, simulating real-world transaction scenarios.
Event Hubs for Ingestion: The generated transaction data is streamed into Azure Event Hubs to simulate real-time ingestion of transactions.
Real-time Processing with Stream Analytics: Azure Stream Analytics processes and analyzes the streaming data in real time, detecting potential fraud or anomalies.
Data Storage: The processed transaction data is saved in Azure Data Lake Storage for further analysis and historical records.
Data Transformation: The saved data is transformed using Azure Databricks, where ETL (Extract, Transform, Load) processes clean and prepare the data for further analysis.
Visualization: The transformed data is loaded into Power BI for data visualization, where insights on transaction patterns, anomalies, and fraud detection are presented in interactive dashboards.

Architecture Workflow;
Data Generation: A Jupyter Notebook (data_generator.ipynb) generates synthetic transaction data (including both fraudulent and normal transactions) and streams it into Azure Event Hubs.
Real-time Stream Processing: The transaction data is ingested by Azure Stream Analytics, which processes the data and applies rules to detect potential fraud.
Storage in Data Lake: The processed data is written to Azure Data Lake Storage for long-term storage.
Data Transformation: Azure Databricks is used to perform data transformations, cleaning the raw transaction data and preparing it for reporting.
Power BI Visualization: The cleaned data is loaded into Power BI, where dashboards provide insights into transaction patterns, fraud occurrences, and trends.

Technologies Used
Jupyter Notebook (Python): For generating synthetic transaction data.
Azure Event Hubs: Streaming service to ingest transaction data in real-time.
Azure Stream Analytics: Real-time processing to analyze transaction streams and detect fraud.
Azure Data Lake Storage: Scalable storage for transaction data.
Azure Databricks: Data engineering platform used for cleaning and transforming transaction data.
Power BI: For visualizing the insights and trends from the transaction data.

Setup Instructions
Prerequisites:

Jupyter Notebook and Python 3.x installed on your local machine.
Azure account with access to Event Hubs, Stream Analytics, Data Lake, Databricks, and Power BI.
Jupyter Notebook Script:

Open jupyter notebook to generate synthetic transaction data and stream it into Azure Event Hubs.
Event Hubs Setup:

Configure an Azure Event Hub to ingest the streaming data.
Stream Analytics Setup:

Set up a Stream Analytics Job to process the incoming data from Event Hubs and apply your business logic for fraud detection.
Data Lake Setup:

Store the processed data in Azure Data Lake Storage for further analysis.
Databricks Transformation:

Use Azure Databricks to perform ETL on the stored data, cleaning and preparing it for visualization.
Power BI Visualization:

Connect Power BI to your transformed data in the Data Lake, and create dashboards to visualize transaction patterns and detect fraud trends.

Future Enhancements
Integrate machine learning models in Databricks to improve fraud detection accuracy.
Implement alerting mechanisms when potential fraud is detected.
Extend the solution to support batch processing alongside real-time processing.

# note: Because I used azure free subscription and having exceeded my access limits while creating another project I do not have access to my resources other than the notebooks and visualations I uploaded
