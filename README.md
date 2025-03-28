# Interactive-Dashboard-for-Chronic-Pain-Management
Designing an interactive dashboard for chronic pain management 

## Introduction
For the design of an interactive dashboard for chronic pain management, relevant datasets from the NHANES 1999-2000 survey were identified and selected. Information on analgesic pain relievers, occupation, miscellaneous pain, medical conditions, and general health status was included in the datasets. The column names in each dataset were then examined to determine the fields most relevant to chronic pain management, such as pain intensity, duration, use of pain relievers, and general health condition. This process ensured that the focus was placed on the most pertinent data for the creation of a comprehensive and insightful dashboard.

After the relevant fields were identified, the datasets were loaded and merged using Python and the Pandas library. All datasets were ensured to be merged on a common identifier (SEQN) to maintain data integrity. Fields from each dataset were combined through the merging process, resulting in a unified dataset containing the most crucial information for chronic pain management. A robust foundation for analyzing and visualizing chronic pain data was provided by this comprehensive dataset.

To enhance the readability of the dataset, the coded field names were replaced with their corresponding descriptive names. This step was deemed crucial for making the dataset more user-friendly and easier to interpret. The final merged dataset was saved as a CSV file, which can be utilized to design an interactive dashboard offering valuable insights into chronic pain management.


## Data Preprocessing

1. SEQN was defined as numerical.
2. All other fields were ensured to be treated as categorical.
3. The preprocessed dataset was saved.

## Key Metrics for Monitoring Pain Levels and Tracking Treatment Outcomes

For the generation of key metrics to monitor pain levels and track treatment outcomes using the categorical data, the preprocessed dataset was loaded, and all relevant fields were ensured to be treated as categorical variables. The percentage distribution of responses within each category was calculated for each metric. For example, the "Average Pain Intensity" was determined by calculating the percentage of respondents who reported different levels of pain intensity, such as "Very mild," "Mild," "Moderate," etc. This same approach was applied to other metrics, including "Pain Duration" (where the percentage distribution of reported pain duration was calculated), "Pain Location" (where the percentage distribution of pain locations was calculated), "Pain Interference with Activities" (where the percentage of days pain interfered with usual activities was calculated), and "General Health Condition" (where the percentage distribution of self-reported general health conditions was calculated).

For treatment outcomes, the "Use of Pain Relievers" was determined by calculating the percentage of patients who reported using pain relievers. The "Frequency of Pain Reliever Use" was found by calculating the percentage distribution of the number of days pain relievers were used in the past month, allowing common usage patterns among patients to be understood. A comprehensive set of metrics that can be visualized in Tableau to effectively monitor and track pain levels and treatment outcomes was created by using these percentage distributions.

## Explanation of the Metrics Calculation
Average Pain Intensity: The percentage of each pain intensity level was calculated.

* Pain Duration: The percentage of each pain duration category was calculated.
* Pain Location: The percentage distribution of pain locations was calculated.
* Pain Interference with Activities: The percentage of the number of days pain interfered with activities was calculated.
* General Health Condition: The percentage distribution of general health conditions was calculated.
* Use of Pain Relievers: The percentage of patients using pain relievers was calculated.
* Frequency of Pain Reliever Use: The percentage distribution of the number of days pain relievers were used in the past month was calculated.


## Interactive Dashboard

The interactive dashboard for chronic pain management was designed using Tableau, with the preprocessed dataset being imported as the primary data source. Various visualizations were created to represent the key metrics effectively.

Two specific visualizations from the dashboard were included to provide deeper insights into chronic pain management. The first visualization, titled "General Health," was a set of bar charts and histograms illustrating the relationship between general health conditions, pain duration, and pain reliever use. The "General Health Condition" bar chart showed the percentage distribution of self-reported health conditions among respondents, with 54.72% reporting "Very good" health and only 1.89% reporting "Poor" health when currently taking pain relief products, compared to 49.54% "Very good" and 15.00% "Poor" among those not taking products. This highlighted that individuals using pain relievers generally reported better health, possibly due to effective pain management. The "Pain Duration" histogram revealed that most respondents (56.67%) experienced pain for "Greater than 1 year," with only 5.66% reporting pain for "Less than 1 month," indicating a prevalence of chronic pain. Additional histograms for "Symptoms begin only because of injury" and "Symptoms present for most of the month" showed that 92.98% of respondents did not attribute their symptoms solely to injury, and 70.20% experienced symptoms most of the month, underscoring the persistent nature of their pain.

![Dashboard 1 (2)](https://github.com/user-attachments/assets/0a6c60b9-afc3-4f14-923c-798010f736eb)
![Dashboard 1](https://github.com/user-attachments/assets/9f02a979-0249-4a92-8c60-e35e9fe491d5)

The second visualization, titled "Use of Pain Relievers" and "Frequency of Pain Reliever Use," was designed to provide insights into the prevalence and patterns of pain reliever usage. A pie chart for "Use of Pain Relievers" was created, showing that 76.04% of respondents did not use pain relievers, 23.71% used them, and 0.22% refused to answer, with 0.04% unsure ("Don't know"). This indicated that a significant majority of respondents did not rely on pain relievers, possibly due to mild pain or alternative management strategies. A bar chart for "Frequency of Pain Reliever Use" was implemented, displaying the percentage distribution of the number of days pain relievers were used in the past month across categories: 50.13% used them for 19-20 days, 23.73% for 21-22 days, 20.25% for 23-24 days, 3.57% for 25-26 days, 1.34% for 27-28 days, 0.62% for 29-30 days, and 0.36% were unsure ("Don't know"). This visualization highlighted that among users, the most common usage pattern was 19-20 days, suggesting frequent but not daily use for many.

![Tracking treatment outcomes](https://github.com/user-attachments/assets/66e820c4-b35c-4854-8f38-2db6e3eff845)

The third visualization, covering "Pain Intensity," "Pain Location," "Pain Duration," and "General Health Condition," was designed to offer a comprehensive view of pain characteristics. A bar chart for "Pain Intensity" was created, showing the average pain intensity across categories (No pain, Very mild, Mild, Moderate, Severe, Very severe), with "Mild" being the most common, followed by "Moderate," indicating that most respondents experienced manageable pain levels. A bar chart for "Pain Location" was implemented, revealing that the lower back was the most common pain location (30.04%), followed by the upper back (18.39%), shoulders (16.59%), and arms (15.70%), with smaller percentages for hands, hips, head, neck, and feet, providing insight into the most affected body areas. A bar chart for "Pain Duration" confirmed that "Greater than 1 year" was the most prevalent duration, aligning with the first visualization’s findings on chronic pain. A bar chart for "General Health Condition" mirrored the earlier visualization, showing "Very good" as the most common health status, reinforcing the trend of relatively good health among respondents despite chronic pain. A pie chart for "Pain Location" was also included, visually summarizing the distribution of pain locations in a circular format, emphasizing the dominance of lower back pain.

![Monitoring pain levels](https://github.com/user-attachments/assets/11d4af22-1afd-4e8c-9fb5-1f129ce44e01)
