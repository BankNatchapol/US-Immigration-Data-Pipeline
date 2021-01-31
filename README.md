[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">

  <h3 align="center">US Immigration Data Pipeline</h3>

  <p align="center">
    Create ETL Data Pipeline using Spark.
    <br />
    <br />
    <a href="https://github.com/BankNatchapol/US-Immigration-Data-Pipeline/issues">Report Bug</a>
    ·
    <a href="https://github.com/BankNatchapol/US-Immigration-Data-Pipeline/issues">Request Feature</a>
  </p>
</p>




<!-- ABOUT THE PROJECT -->
## About The Project

Create an ETL pipeline for I94 immigration, land temperatures, US demographics and airport datasets to form an analytics database on immigration events. A use case for this analytics database is to find immigration patterns to the US. For example, we could try to find answears to questions such as, do people from countries with warmer or cold climate immigrate to the US in large numbers?

The project follows the follow steps:
* Step 1: Scope the Project and Gather Data
* Step 2: Explore and Assess the Data
* Step 3: Define the Data Model
* Step 4: Run ETL to Model the Data
* Step 5: Complete Project Write Up

## Step 1: Scope the Project and Gather Data

### Scope 
- use spark to load data to workspace.
- EDA for checking missing value.
- cleaning data based on EDA result.
- using spark to write parquet file

## Describe and Gather Data 
### I94 Immigration Data
This data comes from the US National Tourism and Trade Office. In the past all foreign visitors to the U.S. arriving via air or sea were required to complete paper Customs and Border Protection Form I-94 Arrival/Departure Record or Form I-94W Nonimmigrant Visa Waiver Arrival/Departure Record and this dataset comes from this forms.

This dataset forms the core of the data warehouse and the customer repository has a years worth of data for the year 2016 and the dataset is divided by month. For this project the data is in a folder located at ../../data/18-83510-I94-Data-2016/. Each months data is stored in an SAS binary database storage format sas7bdat. For this project we have chosen going to work with data for the month of April. However, the data extraction, transformation and loading utility functions have been designed to work with any month's worth of data.

### World Temperature Data
The World Temperature dataset comes from Kaggle and represents global land temperatures by city.

### U.S. City Demographic Data
This data comes from OpenSoft and contains information about the demographics of all US cities and census-designated places with a population greater or equal to 65,000. Original data comes from the US Census Bureau's 2015 American Community Survey.

### Airport Code Table
This is a simple table of airport codes and corresponding cities.

## Step 2: Explore and Assess the Data
### Exploratory Data Analysis and Cleaning Data contain this visualization steps

#### Visualize World Temperature Data missing values

#### Visualize I94 Immigration Data missing values

#### Visualize U.S. City Demographic Data missing values

#### Visualize Airport Code Table missing values


### Step 3: Define the Data Model
#### 3.1 Conceptual Data Model
<img src="images/datamodel.png">

#### 3.2 Mapping Out Data Pipelines
pipeline steps 
- load the datasets
- cleaning data, missing values
- transform raw data to our data models

### Step 4: Run Pipelines to Model the Data 
#### immigration fact table
#### immigration time table
#### airport table
#### us demograghic table
#### land temperature table

#### Step 5: Complete Project Write Up
* Clearly state the rationale for the choice of tools and technologies for the project.
* Propose how often the data should be updated and why.
* Write a description of how you would approach the problem differently under the following scenarios:
 * The data was increased by 100x.
 * The data populates a dashboard that must be updated on a daily basis by 7am every day.
 * The database needed to be accessed by 100+ people.

<!-- CONTACT -->
## Contact

Facebook - [@Natchapol Patamawisut](https://www.facebook.com/natchapol.patamawisut/)

Project Link: [https://github.com/BankNatchapol/US-Immigration-Data-Pipeline](https://github.com/BankNatchapol/AWS-Data-Warehouse-ETL)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/natchapol-patamawisut
