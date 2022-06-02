# New York Yellow Texi Data in Febrary 2022
=================================================================
## DataScience Term Project
## 1) Source and explanation on the dataset (texts)
The yellow texi records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts. 
The data used in the attached datasets were collected and provided to the NYC Taxi by technology providers authorized under the Taxicab Passenger Enhancement Programs(TPEP/LPEP). 
The trip data was not created by the TLC, and TLC makes no representations as to the accuracy of these data.

+ In this dataset, we are considering only the Yellow Taxi Data for the month of Febrary 2022.<br><br>
+ This dataset can be downloaded from the url below. (2022_February_Yellow Taxi Trip Records.CSV)<br>
    https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page

## 2) Objective of your analysis <br>  (texts; what you want to get by analyzing this dataset)
<u>Providing practical analysis for taxi drivers</u> is the main objective of our data set. <br>Since customer’s taxi demand forecasts are only predictable based on accumulated data, these analyses are very useful for taxi drivers. Based on our analysis, taxi drivers can immediately know where there are many customers at a specific time zone.<br><br>
By analyzing a dataset of approximately 3 million rows, we can see which places are most in customer demand at certain times. Also, you can see which regions have the highest customer demand, not only by time zone but also by day of the week.
<br><br>
Furthermore, with these data, we're going to come up with three more interesting analyses.<br><br>
<u>The first is to analyze the section and time zone where the most tips come out.</u> Tip is an important source of income for New York taxi drivers.  So we're going to analyze the sections and time zones that have the most tips.<br><br>
<u>The second is the trend change analysis in New York City.</u> Based on the last 10 years of data tracking the route of taxis, we can analyze the trend of changing hot places for New Yorkers by organizing sections with high congestion and frequency by year.<br><br>
<u>The third is the trend analysis of destinations by number of passengers.</u> Dataset contains the number of passengers in the taxi. When you take a taxi alone or in groups, the origin and destination can usually have different characteristics. For example, areas where a lot of group guests get on or off may be areas where people are more likely to gather, such as parties, concerts, tourist attractions, and transportation centers. The correlation between these passengers and their location will be shown in the analysis.

## 3) Description on the dataset (statistics, tables, plots, missing values, outliers, ... etc) Make it look nice and readable.

### Attributes
|column_name|description|
|-----------|:-----------|
|VendorID|A code indicating the TPEP provider that provided the record. <br>1 : Creative Mobile Technologies <br>2 : VeriFone Inc.|
|tpep_pickup_datetime|The date and time when the meter was engaged.|
|tpep_dropoff_datetime|The date and time when the meter was disengaged.|
|passenger_count|The number of passengers in the vehicle. This is a driver-entered value.|
|trip_distance|The elapsed trip distance in miles reported by the taximeter.|
|RatecodeID|The final rate code in effect at the end of the trip. <br>1 : Standard rate <br>2 : JFK <br>3 : Newark <br>4 : Nassau or Westchester <br>5 : Negotiated fare <br>6 : Group ride|
|store_and_fwd_flag|This flag indicates whether the trip record was held in vehicle memory before sending to the vendor, aka “store and forward,” because the vehicle did not have a connection to the server.  <br>Y : store and forward trip <br>N : not a store and forward trip|
|PULocationID|TLC Taxi Zone in which the taximeter was engaged.|
|DOLocationID|TLC Taxi Zone in which the taximeter was disengaged.|
|payment_type|A numeric code signifying how the passenger paid for the trip. <br>1 : Credit card <br>2 : Cash <br>3 : No charge <br>4 : Dispute <br>5 : Unknown <br>6 : Voided trip|
|fare_amount|The time-and-distance fare calculated by the meter.|
|extra|Miscellaneous extras and surcharges. Currently, this only includes. the 0.50 dollar and 1 dollar rush hour and overnight charges.|
|mta_tax|0.50 MTA tax that is automatically triggered based on the metered rate in use.|
|tip_amount|Tip amount – This field is automatically populated for credit card tips.Cash tips are not included.|
|tolls_amount|Total amount of all tolls paid in trip.|
|improvement_surcharge|0.30 improvement surcharge assessed trips at the flag drop. the improvement surcharge began being levied in 2015.|
|total_amount|The total amount charged to passengers. Does not include cash tips.|
|congestion_surcharge|It represents the additional cost of New York traffic congestion.|

