# etl-airflow-project
# ETL Pipeline with Apache Airflow and BashOperator

This project demonstrates how to build an ETL (Extract, Transform, Load) data pipeline using **Apache Airflow** and the **BashOperator**. It was completed as part of the [IBM ETL and Data Pipelines with Shell, Airflow and Kafka](https://www.coursera.org/learn/etl-data-pipelines-shell-airflow-kafka) course on Coursera.

## 📁 Project Structure

The DAG executes a multi-step ETL process on toll data using shell commands. Tasks include unzipping, extracting data from different formats, consolidating, and transforming it.

### 🔄 DAG Workflow

1. **unzip_data** – Extract compressed `.tgz` data file
2. **extract_data_from_csv** – Extract specific fields from a `.csv` file
3. **extract_data_from_tsv** – Extract fields from a `.tsv` file
4. **extract_data_from_fixed_width** – Extract fields from a fixed-width text file
5. **consolidate_data** – Combine the data from all sources into one `.csv`
6. **transform_data** – Transform the `vehicle_type` column to uppercase

## 🛠️ Technologies Used

- Apache Airflow
- BashOperator
- Bash shell commands (`cut`, `tr`, `paste`, `tar`)
- Python 3.x
- Linux-based environment

## 📸 Screenshots

> Note: These screenshots were taken during development and submitted to Coursera for peer review.

## Screenshots

### DAG Arguments
![DAG Arguments](./screenshots/dag_args.jpg)

### DAG Definition
![DAG Definition](./screenshots/dag_definition.jpg)

### Unzip Data Task
![Unzip Data Task](./screenshots/unzip_data.jpg)

### Extract CSV Task
![Extract CSV Task](./screenshots/extract_data_from_csv.jpg)

### Extract TSV Task
![Extract TSV Task](./screenshots/extract_data_from_tsv.jpg)

### Extract Fixed Width Task
![Extract Fixed Width Task](./screenshots/extract_data_from_fixed_width.jpg)

### Consolidate Data Task
![Consolidate Data Task](./screenshots/consolidate_data.jpg)

### Transform Data Task
![Transform Data Task](./screenshots/transform_data.jpg)

### Task Pipeline
![Task Pipeline](./screenshots/task_pipeline.jpg)

### DAG Submission
![Submit DAG](./screenshots/submit_dag_2.jpg)

### Unpause & Trigger DAG
![Unpause Trigger DAG](./screenshots/unpause_trigger_dag.jpg)

### DAG Tasks List
![DAG Tasks](./screenshots/dag_tasks_2.jpg)

### DAG Runs
![DAG Runs](./screenshots/dag_runs.jpg)


## ▶️ How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/etl-airflow-project.git
   cd etl-airflow-project
