# nyc-yellow-trip-data-pipeline

## Phase 1
In this phase of the project, I will focus on ingesting 1 million rows of data from the NYC Yellow Taxi dataset provided to you. The
goal is to create a robust data pipeline that can efficiently handle and store the dataset for subsequent analysis. You are required to
perform the following tasks:

#### Download and Familiarize:
1. Download the NYC yellow_tripdata_2016-02 dataset and become familiar with its structure and attributes.
2. Data Transformation:
Perform basic data transformation tasks, such as handling data type conversions, to ensure the ingested data is ready for analysis.
3. Data Ingestion:
Implement a data ingestion process to load 1 million rows of data from the dataset into your postgres database system. Ensure that the ingestion process is efficient and can handle large volumes of data.

## Phase 2
In this phase, I will utilize the ingested data to build reporting pipelines that generate valuable insights from the NYC Yellow Taxi dataset. I will create three reporting tables as described below:

#### operations_and_performance
1. How many trips were recorded in the dataset?
2. What is the average trip distance for all trips?
3. Which Vendor has the highest number of trips?
4. Which Vendor has the lowest number of trips?
5. What is the average passenger count per trip?

  Table: ingestion_date | total_trips | avg_trip_distance |highest_trip_vendor | lowest_trip_vendor |

#### customer_demographics_and_preferences
1. What is the average trip amount given by passengers?
2. What is the average trip distance by passengers?
3. How many trips were flagged as 'store and forward'?
4. How many trips were shared rides (passenger count > 1)?
 
  Table: ingestion_date |avg_tip_amount |avg_trip_distance_by_passenger |store_and_forward_trips |shared_ride_count

#### financial_performance
1. What is the average fare amount per trip?
2. How much revenue was generated from tolls and surcharges combined?
3. What is the average total amount paid by passengers?
 
  Table: ingestion_date | avg_fare_amount | tolls_and_surcharges_revenue | avg_total_amount
