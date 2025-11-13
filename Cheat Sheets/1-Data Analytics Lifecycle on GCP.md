# Data Analytics Lifecycle on Google Cloud - Cheat Sheet

## **Core Concepts**

- **Data is essential** for driving innovation, differentiation, and unlocking AI value

- **Data sources** include operational systems, web sources, social media, and IoT devices

- **Data types** can be structured or unstructured—must combine and analyze all types regardless of format

- **Data analytics lifecycle** is an iterative process of collecting, storing, processing, and analyzing data to extract insights

## **The Four Main Stages**

### **1. INGEST**
- **Purpose**: Break down data silos and reduce time to insight

- **Key products**:
  - **Pub/Sub**: Streaming ingestion and messaging
  - **Dataflow**: Streaming analytics and processing
  - **Dataproc**: Batch processing
  - **Cloud Data Fusion**: Code-free ETL tool for integrating on-premises and cloud data

### **2. PROCESS**
- **Transform and prepare** data after ingestion

- **Processing options**:
  - Dataproc for batch processing
  - Dataflow for streaming data
  - Cloud Data Fusion for multi-source integration

### **3. STORE**
- **Requirements**: Secure storage that scales with data growth

- **Storage categories**: Databases, data lakes, and data warehouses

- **Key products**:
  - **Relational databases**: Cloud SQL, Cloud Spanner, AlloyDB for PostgreSQL
  - **NoSQL databases**: Bigtable, Firestore
  - **Data warehouse**: BigQuery
  - **Object storage**: Cloud Storage

### **4. ANALYZE**
- **BigQuery**: Core data warehouse solution—elastic, flexible, secure, cross-cloud, SQL-based

- **Visualization tools**: Looker and Looker Studio for analyzing and visualizing results

- **Machine learning platform**: Vertex AI (includes AutoML, Vertex AI Workbench, TensorFlow)

## **Key Takeaways**

- The lifecycle is **iterative**—expect to move back and forth between steps

- **BigQuery is central** to Google Cloud's data analytics ecosystem

- Google Cloud provides **serverless, comprehensive, and integrated** solutions for each lifecycle stage

- Understanding this lifecycle helps you **identify, prepare, and extract insights** from data effectively