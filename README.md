# YouTube UK Influencers Analytics

An end-to-end data analytics project analyzing the top UK YouTube influencers in 2024.  
Includes Python-based YouTube Data API extraction, SQL data validation, and an interactive Power BI dashboard with ROI and profitability analysis.
![kaggle_to_powerbi](https://github.com/user-attachments/assets/347f3334-d99d-41ec-b281-5b4625ac5f64)

## YouTube Analytics Dashboard – UK Influencers
An end-to-end data analysis project combining **Python**, **SQL**, and **Power BI** to analyze the top YouTube influencers in the United Kingdom for 2024.  
The workflow integrates data from [Kaggle’s Top 100 Social Media Influencers 2024 Countrywise dataset](https://www.kaggle.com/datasets/bhavyadhingra00020/top-100-social-media-influencers-2024-countrywise?resource=download), enriches it with live statistics from the **YouTube Data API**, validates results with SQL, and visualizes insights in an interactive Power BI dashboard.

<img width="1422" height="793" alt="powerbi_dashboard" src="https://github.com/user-attachments/assets/80b79c4b-92dd-40dc-abbe-105a3978972d" />

---

## Project Links
- [View GitHub Repository](<repo-link>)
- [Kaggle Dataset](https://www.kaggle.com/datasets/bhavyadhingra00020/top-100-social-media-influencers-2024-countrywise?resource=download)

---

##  Table of Contents
- [Project Overview](#project-overview)  
- [Project Scope](#project-scope)  
- [Business Objective](#business-objective)  
- [Document Purpose](#document-purpose)  
- [Use Case](#use-case)  
- [Skills Demonstrated](#skills-demonstrated)  
- [Data Source](#data-source)  
- [Data Extraction and Processing](#data-extraction-and-processing)  
- [SQL Data Validation](#sql-data-validation)  
- [Power BI Analysis and Insights](#power-bi-analysis-and-insights)  
- [ROI and Profitability Analysis](#roi-and-profitability-analysis)  
- [Recommendation](#recommendation)  
- [Conclusion](#conclusion)  
- [Built With](#built-with)  
- [Roadmap](#roadmap)  
- [Contact](#contact)  
- [Full Python Script](#full-python-script)   

---

## Project Overview
This project focuses on analyzing YouTube’s most influential UK-based creators. It enhances a publicly available dataset with real-time YouTube API statistics, validates the enriched data in SQL Server, and builds a Power BI dashboard to highlight audience size, content output, and engagement.

---

## Project Scope
- Analyze top UK YouTube influencers in 2024  
- Merge historical influencer data with live YouTube API statistics  
- Validate dataset using SQL checks (row count, columns, schema, duplicates)  
- Create interactive visualizations in Power BI  
- Perform ROI and profitability modeling in Excel  

---

## Business Objective
Deliver data-driven insights into the UK YouTube influencer landscape to support:
- **Marketing Teams** identifying high-reach content creators  
- **Talent Managers** evaluating growth potential  
- **Analysts** tracking platform engagement trends  

---

## Document Purpose
This project demonstrates the integration of Python-based API extraction, SQL data validation, and Power BI reporting in a real-world influencer analytics scenario.

---

## Use Case
**Scenario:**  
A marketing agency is seeking to allocate ad spend to top-performing YouTubers in the UK. They need accurate, up-to-date metrics on subscriber count, views, and content production volume to guide partnership decisions.

---

## Skills Demonstrated
- Python (API integration, data transformation)  
- SQL Server (data validation & transformation)  
- Power BI (data modeling, DAX measures, interactive visuals)  
- Excel (ROI calculations & profitability analysis)  
- GitHub documentation & project organization  

---

## Data Source
- **Provider:** [Kaggle – Top 100 Social Media Influencers 2024 Countrywise](https://www.kaggle.com/datasets/bhavyadhingra00020/top-100-social-media-influencers-2024-countrywise?resource=download)  
- **Format:** CSV  
- **Subset Used:** UK YouTube influencers only  

---

## Data Extraction and Processing
1. Filtered UK YouTube influencers from Kaggle dataset  
2. Extracted channel handles from `NOMBRE` field  
3. Resolved handles to `channelId` via YouTube Search API  
4. Retrieved live stats (`subscriberCount`, `viewCount`, `videoCount`) from YouTube Data API  
5. Merged API data with original dataset and saved as `updated_youtube_data_uk.csv`

---

## SQL Data Validation
SQL Server queries ensured data completeness and correctness.

1. **Row Count Check**  

<img width="776" height="485" alt="1_row_count_check" src="https://github.com/user-attachments/assets/affb259e-117c-4c7b-a65e-5a9dc86d0895" />

2. **Column Count Check**  
<img width="784" height="552" alt="2_column_count_check" src="https://github.com/user-attachments/assets/c9ed347e-f37e-428a-b267-345b5edc054d" />

3. **Data Type Check**  
<img width="817" height="675" alt="3_data_type_check" src="https://github.com/user-attachments/assets/3cfc8f38-e179-4f7a-82d1-790c2e2d2a3c" />

4. **Duplicate Records Check**  
<img width="804" height="568" alt="4_duplicate_records_check" src="https://github.com/user-attachments/assets/50e23ce2-f624-4ba1-8f32-a99b728bb2ad" />

---

## Power BI Analysis and Insights
The Power BI dashboard presents:
- **Top 10 UK YouTubers by Subscribers**  
- **Top 10 by Views**  
- **Total Videos Produced**  
- **Engagement Ratios**  

<img width="1422" height="793" alt="powerbi_dashboard" src="https://github.com/user-attachments/assets/643286cf-0472-4697-a3ba-590a5f4f39d3" />

---

## ROI and Profitability Analysis
Excel-based ROI models calculated potential revenue and profitability based on audience metrics.

### Total Views Analysis
<img width="1982" height="620" alt="Total Views Analysis" src="https://github.com/user-attachments/assets/898d9861-a3bf-41b5-bc22-d09ae26e27d4" />

### Total Videos Analysis
<img width="1994" height="647" alt="Total Videos Analysis" src="https://github.com/user-attachments/assets/0e3739d5-a002-4f88-b51e-facc1ec5b572" />

### Total Subscribers Analysis
<img width="2004" height="647" alt="total subs analysis" src="https://github.com/user-attachments/assets/a0507f5d-b11b-4e38-9711-42333de68a52" />

---

## Recommendation
- Automate data refresh via the YouTube API on a scheduled basis  
- Include audience engagement metrics (likes, comments) for richer analysis  
- Extend to other platforms from the same Kaggle dataset (Instagram, TikTok, Threads)  

---

## Conclusion
By combining API data extraction, SQL validation, and Power BI visualization, this project delivers a reliable, insight-rich dashboard of UK YouTube influencers.  
It demonstrates the full workflow from a public dataset to actionable analytics.

---

## Built With
- Python (`pandas`, `google-api-python-client`)  
- SQL Server  
- Power BI Desktop  
- Excel  
- Kaggle dataset  

---

## Roadmap
- [ ] Batch API calls to improve efficiency  
- [ ] Add automated API refresh with Airflow or Power Automate  
- [ ] Expand analysis to other countries in the dataset  
- [ ] Integrate sentiment analysis on recent videos  

---

## Contact
Kweku Darko  
**Email:** [kaydarko7@gmail.com](mailto:kaydarko7@gmail.com)  
**LinkedIn:** [Kweku Darko LinkedIn](https://www.linkedin.com/in/kweku-darko-b880b4161/)  
**Portfolio:** [Data Portfolio](https://www.datascienceportfol.io/kaydarko7)  

---

## Full Python Script  

_All data is publicly available and used only for educational and demonstration purposes._

```python
import os
import pandas as pd
from dotenv import load_dotenv
from googleapiclient.discovery import build

# Load environment variables
load_dotenv() 

API_KEY = os.getenv("YOUTUBE_API_KEY")
API_VERSION = 'v3'

# Initialize YouTube API client
youtube = build('youtube', API_VERSION, developerKey=API_KEY)

def get_channel_stats(youtube, channel_id):
    """Fetch channel statistics from the YouTube API."""
    request = youtube.channels().list(
        part='snippet, statistics',
        id=channel_id
    )
    response = request.execute()

    if response['items']:
        data = dict(
            channel_name=response['items'][0]['snippet']['title'],
            total_subscribers=response['items'][0]['statistics']['subscriberCount'],
            total_views=response['items'][0]['statistics']['viewCount'],
            total_videos=response['items'][0]['statistics']['videoCount'],
        )
        return data
    else:
        return None 

# Read CSV into dataframe 
df = pd.read_csv("youtube_data_united-kingdom.csv")

# Extract channel IDs and remove potential duplicates
channel_ids = df['NOMBRE'].str.split('@').str[-1].unique()

# Initialize a list to keep track of channel stats
channel_stats = []

# Loop over the channel IDs and get stats for each
for channel_id in channel_ids:
    stats = get_channel_stats(youtube, channel_id)
    if stats is not None:
        channel_stats.append(stats)

# Convert the list of stats to a DataFrame
stats_df = pd.DataFrame(channel_stats)

# Reset indexes for alignment
df.reset_index(drop=True, inplace=True)
stats_df.reset_index(drop=True, inplace=True)

# Concatenate the dataframes horizontally
combined_df = pd.concat([df, stats_df], axis=1)

# Save the merged dataframe back into a CSV file
combined_df.to_csv('updated_youtube_data_uk.csv', index=False)

print(combined_df.head(10))
