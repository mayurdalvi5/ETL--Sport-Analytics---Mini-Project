# Sports Analytics ETL Project

## Overview

This project is a sports analytics ETL (Extract, Transform, Load) pipeline designed to extract data from a source AWS RDS which is (OLTP system), transform the data using Pandas, and load the transformed data into a destination database (OLAP system) for further analysis. The goal is to process sports performance data to assign a performance score to each individual based on their performance metrics.

## Architecture Flow Diagram

![ETL Project Architecture Flow](/ETL Project Architecture Flow.png/)

## Directory Structure

The project directory contains the following files:

- `extract_transform.ipynb`: Jupyter notebook containing the code for the ETL process.
-  `data_for_oltp_DB.zip` : Extract zip file to get `deliveries.csv`, `Player.csv` and `Player_captain.csv`
- `deliveries.csv`: CSV file with delivery data.
- `Player.csv`: CSV file with player data.
- `Player_captain.csv`: CSV file with player captaincy data.

## Prerequisites

Ensure you have the following installed:

- Python 3.x
- Jupyter Notebook
- Pandas
- MySQL Connector
- SQLAlchemy

## Setup and Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/sports-analytics-etl.git
   cd sports-analytics-etl
   ```
2. **Install Required Packages:**

You can install the required packages using pip:

```bash
  pip install pandas mysql-connector-python SQLAlchemy
  ```
3. **Setup AWS RDS Database:**

  Ensure your AWS RDS (OLTP system) is set up and contains the tables `delivery`, `player`,  and `player_captain` with data loaded from the respective CSV files.

## Summary
  This project provides a comprehensive ETL pipeline for sports analytics, enabling efficient data extraction, transformation, and loading processes. By leveraging Python libraries such as Pandas and SQLAlchemy, the pipeline ensures data integrity and facilitates detailed performance analysis. The detailed instructions and provided Jupyter notebook make it easy for other developers to understand, navigate, and utilize this project for similar ETL tasks.
