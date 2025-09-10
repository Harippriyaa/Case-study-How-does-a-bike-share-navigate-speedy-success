# Case-study-How-does-a-bike-share-navigate-speedy-success
Data Analytics Project done as part of the Google Data Analytics Professional Certificate

This project analyzes **Cyclistic (Divvy) bike-share data** to answer the business problem:

**How do annual members and casual riders use Cyclistic bikes differently, and how can we encourage casual riders to become members?**

The work follows the steps of the Google Data Analytics Capstone case study:
- **Ask** → Define the business task
- **Prepare** → Collect 12 months of Divvy trip data
- **Process** → Clean and transform the data
- **Analyze** → Conduct descriptive analysis and visualizations
- **Share** → Summarize findings with charts and recommendations
- **Act** → Propose strategies to convert casual riders into members


Data Source
Divvy Trip Data: Divvy S3 Dataset Repository [https://divvy-tripdata.s3.amazonaws.com/index.html]
For this project, the files used were September 2024 – August 2025.


Analysis Workflow
1. Load Data
2. Import 12 months of .csv files into a single dataframe.
3. Process Data
4. Convert started_at and ended_at to datetime
5. Create ride_length in minutes and HH:MM:SS
6. Create day_of_week (Excel-style: 1 = Sunday … 7 = Saturday)
7. Filter out rides <1 min or >24 hrs
8. Descriptive Analysis
    Mean and max ride length
    Mode of day_of_week
    Seasonal trends
9. Pivot Tables
    Avg ride length by member type
    Avg ride length by member type × weekday
    Count of rides by member type × weekday
10. Visualizations
    Bar chart: rides by day of week
    Bar chart: avg ride length by user type
    Line chart: monthly trips by user type
    Heatmap: rides by hour × weekday
11. Recommendations
    Target weekday commuters with membership benefits
    Convert weekend casuals with seasonal/monthly memberships
    Use geo-targeted promotions at high casual-use stations
