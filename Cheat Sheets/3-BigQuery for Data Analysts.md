# BigQuery - Data Warehouse Cheat Sheet

## **What is BigQuery?**

- **Fully managed data warehouse**: No infrastructure management—focus on SQL queries, not deployment, scalability, or security

- **Dual service**: Both a fast SQL query engine AND a fully managed storage layer

- **Purpose**: Store transformed data and analyze it for business insights and decision-making

## **Data Warehouse vs. Data Lake**

| Data Lake | Data Warehouse (BigQuery) |
|-----------|---------------------------|
| Raw, unorganized data | Structured, organized data |
| No specified purpose | Ready for advanced querying |
| Unclassified | Used for analysis and reporting |

**Flow**: Data sources → Data lake → Data warehouse (BigQuery) → Analysis & reporting

## **Performance & Scale**

- **Speed**: Query terabytes in seconds, petabytes in minutes

- **Real-world examples**:
  - 350+ PB of data stored (single customer)
  - Queries on 10+ trillion rows
  - 10,000 concurrent queries simultaneously
  - 100+ trillion rows across multiple customers

## **Key Features**

### **1. Two Services in One**
- Storage AND analysis of petabytes of data

- Built-in capabilities: ML, geospatial analysis, business intelligence

### **2. Serverless & Fully Managed**
- Zero resource provisioning required

- No backend server management

- Focus entirely on SQL queries

### **3. Flexible Architecture**
- **Separated compute and storage**: Analyze data in BigQuery or where it lives

- **Federated queries**: Read data from external sources

- **Streaming support**: Continuous data updates

- **Powerful tools**: BigQuery ML, BI Engine

### **4. Pricing Options**
- **On-demand**: Pay per bytes processed + table storage

- **Capacity pricing**: Fixed monthly bill with reserved resources

### **5. Built-in Security**
- **Encryption at rest** by default (no customer action needed)

- Protects data on disks, SSDs, and backup media

### **6. Machine Learning Integration**
- Write ML models directly in BigQuery using SQL

- Seamless export to Vertex AI for advanced ML workflows

- Covers full data-to-AI lifecycle

## **BigQuery Structure & Access Control**
```
Project
  └── Dataset
       └── Table
            └── Columns (and Rows)
```

- **Access control levels**: Project, dataset, table, column, and row

- **Datasets**: Containers for tables

- **Tables**: Contain columns and rows of data

## **Resource Management**

### **Slots (Virtual CPUs)**
- BigQuery automatically calculates required slots per query

- Based on query size and complexity

- Units of computation (CPU + RAM)

### **Dynamic Allocation**
- **Storage**: Allocated as consumed, deallocated when removed

- **Query resources**: Allocated by query type and complexity

- **No minimum commitment**: Pay for actual usage only

- **Default access**: 2,000 slots for query operations (can reserve more)

## **Public Datasets**

- BigQuery provides numerous public datasets for anyone to query

- Example: Wikipedia page metadata (10+ billion rows)

- Great for learning and testing queries

## **BigQuery UI Navigation**

- Access via Google Cloud Console navigation menu

- All resources exist within a **project** (links usage to billing)

- Projects provide security, access control, and billing management

## **Best Use Cases**

✓ Analyzing large datasets efficiently  
✓ Near real-time insights  
✓ Running complex SQL queries on structured data  
✓ Business intelligence and reporting  
✓ Machine learning on large datasets  
✓ Integrating data from multiple sources  

## **Quick Tips**

- No SQL experience? Resources and labs available in training courses

- Start with public datasets to practice

- Leverage built-in ML features before moving to Vertex AI

- Use federated queries to analyze data without moving it