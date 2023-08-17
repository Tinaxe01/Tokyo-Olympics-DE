# Tokyo-Olympics-DE
![Power BI Report](https://github.com/Tinaxe01/Tokyo-Olympics-DE/raw/main/olympic-screenshot.png)

## Link to interactive report
[Tokyo Olympics Report](https://app.powerbi.com/view?r=eyJrIjoiNmU3ODllMTUtYzQwNS00NjE2LWIwN2MtNGIyOGViNWI4MjRiIiwidCI6IjY3NTFiMzkyLTkyZDEtNGNhNi04M2RjLTJhM2EwMzA4M2ViMCJ9)


## Data Processing Workflow

This project involves the extraction and processing of Olympic data from a REST API using Azure Data Factory. The data is initially acquired and stored in its raw format within designated folders in Azure Data Lake Storage Gen2.

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

For any inquiries or support, please reach out to chinyatitb1@gmail.com.


## Table of Contents

- [Project Overview](##project-overview)
- [Features](##features)
- [Getting Started](##getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [Usage](#usage)
- [Data Pipeline](#data-pipeline)

## Project Overview

This data engineering project focuses on the acquisition, processing, transformation, and analysis of Olympic data using a robust cloud-based infrastructure. Leveraging Azure services, the project seamlessly navigates through various stages, from data extraction to the creation of insightful analytics and dashboards.

## Features

1. **Automated Data Extraction**:
   - Utilize Azure Data Factory for automated extraction of Olympic data from a REST API source, ensuring up-to-date data feeds.

2. **Organized Data Storage**:
   - Employ Azure Data Lake Storage Gen2 for structured storage, segregating raw and transformed data into separate containers.

3. **Scalable Data Processing**:
   - Leverage Azure Databricks for scalable data processing, including complex transformations and schema inference.

4. **Flexible Data Transformation**:
   - Implement versatile data transformations in Azure Databricks to meet diverse analytical needs.

5. **Enhanced Data Quality**:
   - Utilize schema inference in Azure Databricks to improve data quality and consistency.

6. **Efficient Data Movement**:
   - Seamlessly transfer data between storage containers using Azure services, minimizing latency.

7. **Interactive Analytics**:
   - Integrate Power BI for interactive dashboards and visualizations based on transformed data.

8. **End-to-End Workflow**:
   - Present a comprehensive data engineering workflow covering extraction, transformation, storage, and analytics.

9. **Cloud-Native Architecture**:
   - Highlight the advantages of a cloud-native architecture, including scalability and managed services.

10. **Collaborative Environment**:
    - Foster collaboration among stakeholders using Azure services for efficient teamwork.

11. **Documentation and Support**:
    - Provide clear setup documentation and user support for a smooth experience.

12. **Continuous Improvement**:
    - Emphasize potential for ongoing enhancement through new data sources, transformations, and analytics.


## Getting Started

Follow these steps to set up and run the Olympic Data Engineering project on your local or cloud environment.

### Prerequisites

- [Azure subscription](https://azure.microsoft.com/)
- [Azure Data Factory](https://azure.microsoft.com/services/data-factory/)
- [Azure Data Lake Storage Gen2](https://azure.microsoft.com/services/data-lake-storage/)
- [Azure Databricks](https://azure.microsoft.com/services/databricks/)
- [Power BI](https://powerbi.microsoft.com/) (optional, for analytics)

### Installation

1. Clone this repository to your local machine or a cloud environment:

   ```bash
   git clone https://github.com/yourusername/olympic-data-engineering.git
   cd olympic-data-engineering

### Configuration

To successfully set up and run the Olympic Data Engineering project, you'll need to configure various components. Here's how to configure the necessary settings:

### Azure Data Factory Configuration

1. **Create Data Factory**: Set up an Azure Data Factory instance in your Azure portal.

2. **Define Data Sources**: Configure data source connections within Azure Data Factory for accessing the REST API containing Olympic data.

3. **Create Pipelines**: Design pipelines to extract data from the REST API and land it in the raw container in Azure Data Lake Storage Gen2.

### Azure Databricks Configuration

1. **Provision Databricks Workspace**: Create an Azure Databricks workspace in your Azure portal.

2. **Data Transformation**: Utilize Databricks notebooks to perform data transformations. Infer schema and apply necessary processing to refine the data.

### Azure Data Lake Storage Gen2 Configuration

1. **Set Up Containers**: Create containers for both raw and transformed data in Azure Data Lake Storage Gen2.

2. **Access Control**: Configure appropriate access control and permissions for the containers to ensure data security.

### Power BI Configuration (Optional)

1. **Connect to Transformed Data**: In Power BI, connect to the transformed data container in Azure Data Lake Storage Gen2.

2. **Build Dashboards**: Design interactive dashboards and visualizations to derive insights from the transformed Olympic data.


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

## Example Workflow

For code examples illustrating ADF pipelines, Databricks notebooks, and Power BI integration, explore the [examples](./examples) directory in the repository.

## Data Pipeline

[If your project involves a data pipeline, explain its components and how data flows through the system.]

---

**Note:** [Add any additional notes or acknowledgments you want to include. This could be credits to external libraries, datasets used, or anything else you think is relevant.]

For questions or support, contact [your contact information].
