# Mainframe-to-Azure-ETL-Pipeline
This project demonstrates a production-ready ETL flow. It moves data from flat-file extracts (Mainframe style) into an Azure SQL Database.
# Azure Data Factory: Incremental ETL Pipeline (Mainframe-to-Cloud)

### Project Overview
I built this project to demonstrate a production-ready **Incremental Load** (Delta) pattern. 
Drawing from my 3.5 years of experience in the Mainframe field, I applied legacy batch 
control concepts to modern Azure Cloud architecture.

### Features
* **Watermarking:** Uses a SQL control table to track the last processed record, 
  ensuring only new data is moved (cost-optimization).
* **Centralized Error Logging:** Implemented a "Red Arrow" path that captures 
  pipeline failures into a dedicated SQL log table.
* **Stored Procedures:** Automates the "Success" and "Failure" scenarios by 
  updating control tables upon task completion.

### Tech Stack
* **Orchestration:** Azure Data Factory (ADF)
* **Storage:** Azure Data Lake Storage (ADLS) Gen2
* **Database:** Azure SQL Database
* **Logic:** T-SQL, JSON Expressions

### Proof of Success
![Pipeline Success Screenshot](path_to_your_image.png)
