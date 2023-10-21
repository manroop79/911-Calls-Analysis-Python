# 911-Calls-Analysis-Python

## Table of Contents

- [Project Overview](project-overview)
- [Data Sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-(EDA))
- [Data Analysis](#data-analysis)
- [Visualizations](#visualizations)
- [Results](#results)
- [Limitations](#limitations)
- [References](#references)

## Project Overview
This project focuses on an in-depth analysis of the 911 calls dataset, aiming to uncover patterns, trends, and insights related to emergency calls in a metropolitan area. By leveraging data exploration, visualization, and analysis techniques, the project provides a comprehensive understanding of the nature and dynamics of emergency services in the specified region.
![Project Overview Image](https://raw.githubusercontent.com/manroop79/911-Calls-Analysis-Python/main/visualization.png)

## Data Sources
The dataset used for this analysis was obtained from 911.csv. It comprises a comprehensive record of emergency calls, including information such as call type, location, and time, providing valuable insights into the nature of emergencies and the corresponding response mechanisms.

## Tools Used
The analysis was conducted using the following tools and technologies:

- Python
- Jupyter Notebooks
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Data Cleaning and Preprocessing

The dataset underwent a series of preprocessing steps to ensure data consistency and integrity. The data cleaning process primarily involved the following key steps:

### Conversion to Datetime Format

To enable time-based analysis, the 'timeStamp' column in the dataset was converted to the datetime format using the `pd.to_datetime()` function from the pandas library. This conversion facilitated the extraction of various time-related components for further analysis.

### Extraction of Time Components

Further, the following time components were extracted from the 'timeStamp' column to provide additional insights into temporal patterns and trends:

- **Hour:** The hour of the day was extracted using the `.dt.hour` attribute to understand the distribution of calls throughout the day.
- **Month:** The month was extracted using the `.dt.month` attribute to identify any seasonal variations or patterns in the emergency calls data.
- **Day of Week:** The day of the week was extracted using the `.dt.dayofweek` attribute and mapped to corresponding day names (e.g., Monday, Tuesday) to analyze weekly trends in emergency call volumes.

These preprocessing steps were instrumental in preparing the dataset for exploratory data analysis and deriving meaningful insights regarding the temporal dynamics of emergency calls.

## Exploratory Data Analysis (EDA)
The exploratory data analysis phase involved a thorough examination of the dataset to identify key trends, patterns, and correlations. Various statistical and visual exploration techniques were employed to gain insights into the distribution and characteristics of the 911 calls data.

## Data Analysis
Building upon the insights derived from the EDA, the data analysis stage delved deeper into uncovering underlying relationships and associations within the dataset. Advanced analytical techniques were utilized to derive meaningful interpretations and draw actionable conclusions.

## Visualizations
To facilitate a comprehensive understanding of the data, a variety of visualizations such as bar plots, histograms, heatmaps, and clustermaps using seaborn and plots using Matplotlib were generated. These visual representations effectively conveyed complex information and trends in a visually appealing and accessible manner.

## Results
1. The analysis revealed crucial insights into the patterns of emergency calls, response times, peak hours, and prevalent types of emergencies within the metropolitan area.
2. Emergency Medical Services (EMS) was the reason responsible for the highest number of 911 calls.
3. Most calls were made between the time frame of 4-6 pm.
4. These findings contribute to a better understanding of the dynamics of emergency services and can aid in the optimization of response strategies.

## Limitations
- It's important to note certain limitations within the scope of this analysis. Factors such as data availability, data quality, and the specific context of the dataset may have influenced the results and should be considered when interpreting the findings.
- Also to facilitate a comprehensive analysis of the data, the day names extracted from the 'timeStamp' column were mapped to numerical values. This process allowed for a standardized representation of the days of the week, aiding in the analysis of weekly trends and patterns. The following mapping was applied to convert the textual day values to numerical representations:

## References
- Stack Overflow
- ChatGPT
