Billboard Hot 100 Songs Analysis
Project Overview
This project focuses on analyzing the Billboard Hot 100 Songs dataset using OLAP (Online Analytical Processing) techniques. The primary goal was to process and aggregate data to gain insights into the rankings of songs and artists over time.

Dataset
The dataset used in this project is the Billboard Hot 100 Songs dataset, which includes information such as song names, artists, rankings, and dates.

File Path: /kaggle/input/billboard-the-hot-100-songs/charts.csv
Key Columns:
Artist
Song Name
Date
Rank
Indicator (C5) - Set to 1 for all records
Steps and Procedures
1. Loading and Preparing the Data
The dataset was initially loaded and processed using PySpark to perform transformations and create a data cube. This allowed for the aggregation of data by artist, song, and date to analyze trends in the Billboard rankings.

2. Data Import and Schema Adjustment
After creating the data cube, it was imported into SQLite using the DataGrip IDE. During this process, the schema was adjusted, particularly converting the Date column from a TEXT type to a DATE type to facilitate time-based queries and analysis.

3. OLAP Operations
A series of OLAP operations were performed to explore the dataset:

Slicing: Focused on specific artists, such as Taylor Swift, to analyze their song rankings.
Dicing: Created sub-cubes by filtering data across multiple dimensions, such as artist and specific date ranges.
Drill Down: Provided detailed analysis by breaking down the data into more granular levels, like individual song performance over time.
Drill Up (Roll Up): Aggregated data to a higher level, allowing for an overview of overall artist performance.
Advanced OLAP Techniques: Pivoted data, utilized window functions for ranking, and emulated cube operations to uncover deeper insights.
4. Results and Insights
The analysis revealed patterns in song and artist performance over time. By leveraging OLAP operations, it was possible to gain a comprehensive understanding of how songs ranked on the Billboard Hot 100, particularly focusing on key artists.

Tools and Technologies
PySpark: For initial data processing and cube creation.
SQLite & DataGrip IDE: For database management and executing OLAP queries.
Kaggle Notebook: Used for data manipulation and running PySpark scripts.
How to Use
Load the Dataset: Download and load the dataset for processing.
Run Data Processing: Execute the necessary steps to create a data cube and import it into SQLite.
Perform OLAP Queries: Use the provided OLAP operations to explore and analyze the dataset.
License
This project is licensed under the MIT License.

Acknowledgements
Kaggle: For providing the Billboard Hot 100 Songs dataset.
JetBrains DataGrip: For the IDE used in database management.
