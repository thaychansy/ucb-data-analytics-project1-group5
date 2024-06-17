# UCB-DATA-ANALYTICS-PROJECT1-GROUP5

<img width="260" alt="image" src="https://github.com/thaychansy/ucb-data-analytics-project1-group5/assets/161902555/f32948dc-74cf-46c8-aa4c-b7eaabb7970e">


**#Title: Google Top 10 Big Query Search Terms**

Team members: Iosif V., Scott J., Thay C., Krutika D.

The scope of this project was to identify a relationship between top 10 search terms in a popular search engine like google and explore any relevant trend to ongoing world events. The sample dataset <insert link> of 100K records in the Google Biquery Search Database. The date range for data points was narrowed to Jan2024 to May2024 for ease of exploration. Total of 6 search categories - Entertainment, Holidays, News, Public Figures, Sport and Technology were identified for the purpose of this exploratory data set.
Aim of this exploratory analysis was to identify trends for below questions:
1. What are the Top Ten Google search Categories? What are the Top Search Terms used for these Categories?
2. What do these Top serach term results say about trends of search by DMA regions? Is there a preference in search teram by region?
3. Within the idetified top category (i.e. Sports), what were the top terms used?
4. What insights can we glean from the top search term results, region preference and category distribution?

The data analysis approach was structured into the following steps:


We began by selecting the dataset, converting it into a CSV file, and exporting the reads into an Excel worksheet for visualization of its contents. Following this approach, we successfully developed a prototype for testing the hypothesis and identified the specific column headers to use for subsequent querying.The identified areas of interest were divided into worksheets, and exploratory analysis was conducted. The dataset mapping file has been uploaded to the Git repository for reference. Once we identified trends, we narrowed down our search criteria to include data points with higher population to create visualizations in Visual Studio Code using pandas.

**Data points queried as follows:**
1. Which was the category that had most search terms? SPORTS
2. What was the trend of category of serach terms across regions? SPORTS searched most in SOUTH
3. What were the top 10 search terms in the SPORTS category? MAVS/CELTICS/KNICKs
4. Which were the Top 3 regions for these serach terms? Mid W. - CELTICS, NE - MAVS, SOUTH - MAVS, WEST - KNICKS
5. Further instigating the distribution for serach of CELTICS by region - top search in SOUTH.
6.  Search trend distribution by WEEK - March 24 shows peak in trend
7. What was the number one search term for this category - HARISON BUTKER.
HARISON BUTKER was searched the most in NY.
CELTICS was searched the highest in TX.
KNICKS was searched the highest in NY.

**SUPPORTING FILES AND FOLDERS IN GIT REPOSITORY:**

A. Google_Bigquery_Top_Search_Jan_Jun_2024.xls - primary file corted from CSV to be used as source for coding.
This file contains mutiple worksheets to break down the serach criteria used to query the dataset.

B. Google_Biquery_Top_Search_Week_Ending_2024-06-02.csv - excel file used to narrow down search results for certain window.

C.Google_Biquery_Long_Lat.csv - Longitude and Latitude tags were added to be able to indentify the regions from where the serach terms were enetered in search engine.

D.NBA 23-24 Records by Teams, by Month - Merge Candidate.csv - additiona reference dataset downloaded and normalized to see if this could be used to futher evaluate teams score and rankings around the time these search terms were trending to evluate relationship. Topic was eliminated since team ran out of time.

E. Slide Deck used for Class presentation

F. Summary 

# Link to Presentation
https://docs.google.com/presentation/d/1PAC4UgnpjgXocBDq-0srVPpcNn_Tnr6CELcISpCxTmA/edit?usp=drive_link




