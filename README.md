# **Airflow + GCP + BigQuery: ELT Pipeline & Reporting**

This project demonstrates an end-to-end ELT orchestration using **Apache Airflow**, hosted on a **Google Cloud VM**, to load data from **Google Cloud Storage (GCS)** into **BigQuery**, apply transformations, create reporting views, and visualize insights via **Looker Studio**.


### 🔧 **Tech Stack:**

* **Apache Airflow** (on GCP Compute Engine)

* **Google Cloud Storage (GCS)**

* **BigQuery** (Staging, Transformed, and Reporting datasets)

* **Looker Studio** (for final reporting)


### ✅ **Key Features:**

* Cloud-native ELT pipeline using Airflow and GCP

* Sensor-based file existence check before loading

* Staging-to-transformed-to-reporting data flow

* Country-specific BigQuery table creation

* Filtered view generation for optimized reporting

* Final dashboard built using Looker Studio


### 📁 **Project Components:**

* **Airflow DAGs**

  * _dag1.py_ : Basic CSV load from GCS to BigQuery

  * _dag2.py_ : Adds sensor to wait for file availability

  * _dag3.py_ : Creates country-level tables in _transformed_dataset_

  * _dag4.py_ : Generates clean views in _reporting_dataset_

* **BigQuery Datasets**

  * _staging_dataset_, _transformed_dataset_, _reporting_dataset_

* **GCS bucket:** Source CSV file


### 📊 **Output:**

The final dashboard is built in Looker Studio using BigQuery views, showing disease-specific statistics by country, year, and category with key metrics like prevalence and incidence rates.


### 📄 **Full Setup Guide:**

For the detailed, step-by-step setup including environment, configurations, errors, and resolutions **— refer to the PDF guide included in this repository.**

