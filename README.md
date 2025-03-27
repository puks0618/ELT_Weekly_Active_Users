# Weekly Active Users (WAU) Chart Project

## Overview
This work focuses on creating a Weekly Active Users (WAU) chart using modern data engineering tools including Airflow for ETL/ELT processes.

## Project Components
### 1. Data Sources
- `user_session_channel`: Raw user session data
- `session_timestamp`: Timestamp information for sessions

### 2. ETL DAG (Extract, Transform, Load)
#### Objectives
- Import raw tables from Snowflake
- Perform initial data extraction
- Prepare data for further analysis

#### Key Steps
- Connect to Snowflake data source
- Extract `user_session_channel` and `session_timestamp`
- Load data into staging area

### 3. ELT DAG (Extract, Load, Transform)
#### Objectives
- Join raw tables
- Create `session_summary` table in analytics schema
- Implement data quality checks

#### Transformation Logic
- Join `user_session_channel` and `session_timestamp`
- Aggregate session data
- Detect and handle duplicate records

### 4. Visualization
- Create WAU (Weekly Active Users) chart
- Analyze user engagement trends

## Technical Stack
- Airflow: Workflow orchestration
- Snowflake: Data warehouse

## Data Flow
1. Raw Data Ingestion (ETL DAG)
2. Data Transformation (ELT DAG)
3. Analytics Table Creation
4. Visualization Generation

## Additional Notes
- Duplicate record detection implemented
- Weekly aggregation of user sessions
- Comprehensive data quality checks

## Setup Instructions
1. Configure Snowflake connection
2. Set up Airflow DAGs
3. Verify data transformations
4. Create WAU visualization

## Screenshots
- ETL DAG Screenshot: ![image](https://github.com/user-attachments/assets/1dfaf9e4-e1d7-4d3a-a4ab-cea36e438159)

- ELT DAG Screenshot: ![image](https://github.com/user-attachments/assets/b4a7532b-e915-431d-8c13-6d6d7a22dd3a)

