**Analysis of 2020 US Ultra-Marathon Performance**


**Project Overview**

This project performs an exploratory data analysis on a large dataset of ultra-marathon running records. The goal is to investigate performance trends by focusing on races that occurred in the USA during 2020 with distances of either 50km or 50 miles.

The dataset can be found here: https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running/discussion/420633

**Data Cleaning and Preparation**

The initial dataset contained over 7.4 million records. The following steps were taken to clean and prepare the data for analysis:

  1. Filtered the data to include only records from the year 2020, with race lengths of '50km' or '50mi'.

  2. Isolated events that took place in the USA by extracting the country code from the 'Event name' column.

  3. Created an athlete_age column by subtracting the 'Athlete year of birth' from 2020.

  4. Cleaned and standardized column names (e.g., 'Year of event' to year).

  5. Removed irrelevant columns and dropped rows with null values to ensure data quality.

  6. Corrected the data types for numerical columns like athlete_age and athlete_average_speed.

**Key Findings & Analysis**

After cleaning and preparation, two primary questions were investigated:

**1. How does average speed differ between male and female runners?**

  Analysis shows that, on average, male athletes recorded a higher average speed than female athletes in both the 50km and 50-mile distances.

  50km Race: Males (7.74 km/h) were about 9.2% faster than females (7.08 km/h).

  50-mile Race: Males (7.26 km/h) were about 6.2% faster than females (6.83 km/h).

  This difference is clearly visualized in the violin plot below, which shows the distribution of speeds for each group.

**2. Does the race season have an impact on average performance?**

  To analyze seasonal impact, the race month was extracted and categorized into four seasons. The analysis shows a clear difference in average speeds across the seasons.

  Spring: 7.68 km/h (Fastest)

  Winter: 7.52 km/h

  Fall: 7.41 km/h

  Summer: 6.87 km/h (Slowest)

  The slowest average speeds were recorded during the summer months, which may be attributed to hotter and more challenging race conditions. The fastest times were in the spring.

**Tableau Dashboard**

<img width="1723" height="1009" alt="Screenshot 2025-07-27 at 12 30 22 PM" src="https://github.com/user-attachments/assets/9b706cfe-69ad-4d30-bad1-0389ecc98666" />

**Conclusion**
This analysis of 2020 US ultra-marathons reveals clear performance patterns related to athlete gender and race season. Male runners consistently outperform female runners in average speed, and athletes of all genders tend to run significantly slower during the summer.
