# WorldScope-Project

## Colab link:
https://colab.research.google.com/drive/1bD7mZsuIeZ3ZKTdUyIBqXBl0Re8tH8qP?usp=sharing

## Introduction
### Background
This information retrieval system does not merely provide crucial data on global development; it delves into the trends and impacts behind these figures, offering valuable insights to policymakers and researchers.

#### Target User Group:
Policymakers, economists, researchers, academic institutions, non-governmental organizations (NGOs), and the general public.

#### Primary Uses:
• Development Research: Offers socioeconomic indicators analysis for countries worldwide, assisting policy research and decision-making.
• Trend Forecasting: Utilizes historical and current data to predict trends in global economic and social development.

### Data Source Specifications and Procurement Details:
• Worldwide Indicator Data: Sourced from CSV files, this dataset includes socio-economic indicators from countries worldwide, such as population, arable land area, and central government debt.

• Worldwide Project Data: Extracted from SQL Databases, this dataset contains details on World Bank project lending since 1947, including project scale, fund allocation, and completion status.

• World Bank Indicator API: This API provides direct access to updated and comprehensive data on global socio-economic indicators, complementing the information gathered from CSV files and SQL databases.

<img src="assert/Data Lake Architecture Diagram.png" >

### Business idea:
Our architecture is divided into several key components:
• We begin with data extraction, a crucial step in our ETL process. For big data scenarios,
we employ Flume as our extraction tool and Spark for transformation and loading.

• The ETL-processed data is then loaded into our data warehouse. We've chosen Google
Cloud's BigQuery for its stability, user-friendliness, and attractive initial offers.

• Next is data presentation on the user interface, which is powered by a backend Flask API
and crafted with HTML for a seamless user experience.

• Expanding our services, we utilize Google Analytics to dissect user behavior, which
informs our ML recommendation system. This system is designed to bolster our report payment services by providing tailored recommendations.

We've streamlined our system to not only retrieve and process information efficiently but also to engage users with intuitive interfaces and personalized experiences. Then, we will illustrate 3 key parts of our data lake structure.

