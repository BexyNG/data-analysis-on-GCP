# Google Cloud Storage Solutions - Cheat Sheet

## **Data Sources Overview**

- **Definition**: Connectors that let you query data from various sources to create datasets for analysis and ML

- **Two Categories**:
  - **Cloud data sources**: Stored on Google Cloud (e.g., Cloud Storage buckets, Cloud SQL)
  - **External data sources**: Stored on-premises or other cloud providers (e.g., Amazon S3, Microsoft SQL Server)

- **Key Benefits**:
  - Centralized access to data across all locations
  - Easy integration from multiple sources
  - Enables trend analysis and predictions
  - Supports data visualization for actionable insights

## **Storage Options: Three Main Types**

### **1. Databases**
Organized collections of data stored in tables and accessed electronically

#### **Relational Databases** (SQL-based)
- **Products**: Cloud SQL, Cloud Spanner, AlloyDB for PostgreSQL

- **Characteristics**:
  - Data stored in structured rows and columns
  - Use SQL for queries and data manipulation
  - Establish relationships between data points through table joins
  - Highly consistent and reliable
  - Best for large amounts of structured data

#### **Non-Relational Databases** (NoSQL)
- **Product**: Bigtable (also Firestore)

- **Characteristics**:
  - Flexible data model without tabular format
  - No rigid rows and columns structure
  - Ideal for frequently changing data organization
  - Best for diverse data types and applications

### **2. Data Warehouses**
- **Product**: BigQuery

- **Purpose**: Designed specifically for analyzing data (not just storage)

- **Use Case**: Enterprise system for analysis and reporting of structured and semi-structured data from multiple sources

### **3. Data Lakes**
- **Purpose**: Repository for ingesting, storing, exploring, processing, and analyzing raw data

- **Characteristics**:
  - Stores any type or volume of data
  - Keeps data in original format
  - No size limits or pre-processing required
  - Often uses multiple products depending on data nature

## **Data Warehouses vs. Data Lakes**

- **Complementary tools**, not competing solutions

- **Different optimization**:
  - Data warehouses: Optimized for structured data analysis
  - Data lakes: Optimized for raw, diverse data storage

## **Data Types & Use Cases**

### **Structured Data**
- Organized into rows and columns

- **Best for**: Data analytics and statistical analysis

- Well-suited for traditional analysis techniques

### **Unstructured Data**
- Does not fit into tables or spreadsheets

- **Examples**: Text, images, audio

- **Best for**: Machine learning (ML can use both structured and unstructured data)

- ML algorithms learn patterns and make predictions from unstructured data

## **Core GCP Storage Products Summary**

| Product | Type | Best For |
|---------|------|----------|
| Cloud Storage | Object Storage | Data lakes, raw files |
| Cloud SQL | Relational DB | Structured transactional data |
| Cloud Spanner | Relational DB | Global-scale structured data |
| AlloyDB for PostgreSQL | Relational DB | High-performance PostgreSQL workloads |
| Bigtable | NoSQL DB | Large analytical/operational workloads |
| Firestore | NoSQL DB | Document-based applications |
| BigQuery | Data Warehouse | Analytics and reporting |

## **Key Principle**

**Databases** = Store and retrieve data  
**Data Warehouses** = Analyze data  
**Data Lakes** = Store raw data at scale