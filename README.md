# Tokyo-Olympics-DE
Welcome to my project! This repository showcases my work in the field of data engineering, with a focus on Microsoft Azure technologies.
## Tokyo Olympic Report
![Power BI Report](https://github.com/Tinaxe01/Tokyo-Olympics-DE/raw/main/olympic-screenshot.png)

## Link to interactive report
[Tokyo Olympics Report](https://app.powerbi.com/view?r=eyJrIjoiNmU3ODllMTUtYzQwNS00NjE2LWIwN2MtNGIyOGViNWI4MjRiIiwidCI6IjY3NTFiMzkyLTkyZDEtNGNhNi04M2RjLTJhM2EwMzA4M2ViMCJ9)

## About the Project

In this project, I've leveraged my Azure data engineering skills to build a robust data pipeline that ingests, processes, and analyzes large datasets (this is just for demo). My goal is to demonstrate my proficiency in working with Azure's data tools and services.

## Technologies and Skills Showcased

- **Azure Data Factory:** Designed and implemented data workflows using Azure Data Factory to orchestrate data movement and transformations across various sources and destinations.

- **Azure Databricks:** Utilized Azure Databricks for scalable and collaborative data processing. Developed ETL jobs and notebooks for data transformations and analysis.

- **Azure Key Vault:** Leveraged Azure Key Vault to securely manage and store sensitive configuration settings, secrets, and keys used in the data pipeline.

- **Azure Data Lake Storage Gen2:** Utilized Azure Data Lake Storage Gen2 for scalable and high-performance storage of large datasets, seamlessly integrating it into the data pipeline.


## Data Processing Workflow

This project involves the extraction and processing of Olympic data from a REST API using Azure Data Factory. The data is initially acquired and stored in its raw format within designated folders in Azure Data Lake Storage Gen2. We use only 1 copy activity and 2 datasets (source and sink).

![Power BI Report](https://github.com/Tinaxe01/Tokyo-Olympics-DE/raw/main/tokyo-data-pipeline2.png)

### Process Overview

1. **Data Extraction and Landing**:
   - Utilizing Azure Data Factory, the project fetches Olympic data from a REST API source.
   - The acquired data files are deposited into distinct folders within the "raw" container within Azure Data Lake Storage Gen2. Each folder corresponds to the respective data file.

2. **Data Transformation and Schema Inference**:
   - Azure Databricks is employed to execute data transformations and infer the schema.
   - Transformations are performed to refine and shape the data according to specific analytical requirements.
   - The inferred schema enhances the consistency and structure of the data.

3. **Data Sink to Transformed Storage**:
   - After transformation, the processed data files are stored in the "transformed" container in Azure Data Lake Storage Gen2.
   - The "transformed" container holds the refined data, making it readily accessible for analytical purposes.

4. **Analytics and Dashboards**:
   - The transformed data, residing in the "transformed" container, is read and analyzed using Power BI.
   - Power BI facilitates the creation of interactive dashboards and insightful visualizations for in-depth data exploration.

This end-to-end workflow showcases how Olympic data is ingested, processed, transformed, and ultimately made available for analytics and dashboard creation using a combination of Azure services.

## Project Overview

This data engineering project focuses on the acquisition, processing, transformation, and analysis of Olympic data using a robust cloud-based infrastructure. Leveraging Azure services, the project seamlessly navigates through various stages, from data extraction to the creation of insightful analytics and dashboards.


## Getting Started

Follow these steps to set up and run the Olympic Data Engineering project on your local or cloud environment.

### Prerequisites

- [Azure subscription](https://azure.microsoft.com/)
- [Azure Data Factory](https://azure.microsoft.com/services/data-factory/)
- [Azure Data Lake Storage Gen2](https://azure.microsoft.com/services/data-lake-storage/)
- [Azure Databricks](https://azure.microsoft.com/services/databricks/)
- [Power BI](https://powerbi.microsoft.com/) (optional, for analytics)


## Usage

With Azure Data Factory (ADF) as the backbone of the Olympic Data Engineering project, you can efficiently manage data ingestion, transformation, and integration with Azure Databricks for advanced processing. Follow these steps to maximize the benefits of this workflow:

1. **Data Extraction and Ingestion**:
   - Configure Azure Data Factory pipelines to extract Olympic data from the REST API.
   - Utilize ADF's data movement capabilities to load the extracted data into the "raw" container within Azure Data Lake Storage Gen2.

2. **Data Transformation with Azure Databricks**:
   - Set up an Azure Databricks cluster and notebooks to perform intricate data transformations.
   - Trigger the Azure Databricks job within your Azure Data Factory pipeline to seamlessly integrate your transformation logic.

3. **Data Storage and Integration**:
   - Post-transformation, the refined data will be available in the "transformed" container within Azure Data Lake Storage Gen2.

4. **Analytics and Visualization** (Optional):
   - Leverage Power BI to connect to the transformed data stored in the "transformed" container.
   - Generate interactive dashboards, reports, and visualizations to glean insights from the processed data.

5. **Exploration and Refinement**:
   - Experiment with various transformations and visualization techniques to uncover deeper insights.
   - Iterate on your workflow and enhance it based on your evolving analysis goals.

---
**Acknowledgments**: I would like to express my heartfelt appreciation to Darshil Parmar, whose invaluable contributions have significantly enriched the landscape of data engineering. His dedication and expertise have left an indelible mark on this field. A special note of gratitude goes to him for generously providing the dataset and crafting enlightening video tutorials. His efforts have undoubtedly propelled the data engineering community forward, inspiring countless learners along the way.

For questions or support, contact chinyatitb1@gmail.com.
