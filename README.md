# UCB-DATA-ANALYTICS-PROJECT1-GROUP5

<img width="260" alt="image" src="https://github.com/thaychansy/ucb-data-analytics-project1-group5/assets/161902555/f32948dc-74cf-46c8-aa4c-b7eaabb7970e">

# Team Members

- <b>Iosif Vardoev
- Kayla Vaccaro
- Krutika Desai
- Scott Johnson
- Thay Chansy</b>
# Project1 Repository Files
 > <b>CODE FILES (.ipynb) 
1. exploratory_data_analysis_google.ipynb
 
    Description - </b> This file contains code to perform initial cleaning of the Google search data, including an initial attempt to convert to Monthly results and prepare for merging with team-performance (W/L) data
<b>
2. google_bi_query_lt_lg.ipynb
 
    Description - </b> This file ...
<b>
3.  import_weekly_records.ipynb

    Description - </b> This file contains the code that reads in the csv file containing the results of all 82 regular-season games for each of the teams in the search results.  The converts the (W)ins and (L)osses into weekly and season-to-date winning-percentage numbers. 
    <br>Finally, the code reduces the results to one record per week (ending Sunday) of the season to match the search data for merging and further analysis. These records are output to <u>team_weekly_stats.csv</u>
<b>
4.  Add_PO_merge.ipynb

    Description - </b> This file contains the code that first imports the file output from import_weekly_records.ipynb, team_weekly_stats.csv.
    <br>Next, the code imports the the data in <u>NBA Playoff records.csv</u>, converts the days of each game to a week (ending Sunday) and filters to just the five teams in the Google search data.
    <br>Finally, the code merges the playoff results with the regular-season data to form a complete picture of 2024 NBA performance and outputs the result to <u>teams_playoffs.csv</u>
<b>
5.  NBA_search+record_merge.ipynb 

    Description - </b> This file contains code to merge the code to merge the search data with the regular-season and playoff results and.
    <br>The code then performs some statistical analyses on the combined data set.

> <b>DATA Files (.csv) 
1. Google_Bigquery_Top_Search_Jan_Jun_2024.csv
 
    Description - </b> This file contains the weekly search data, by DMA for the top-25 search terms in the United States on Google.com 
<b>
2. Google_Bigquery_Top_Search_Jan_Jun_2024_More_Columns.csv
 
    Description - </b> This file contains the weekly search data, by DMA for the top-25 search terms in the United States on Google.com 
<b>
3. Google_Bigquery_Top_Search_Long_Lat.csv
 
    Description - </b> This file contains the weekly search data, by DMA for the top-25 search terms in the United States on Google.com, updated to include latitude and longitude values.
<b>
4. searched_teams_results.csv
 
    Description - </b> This file contains the regular-season Win/Loss records for the five teams NBA teams (Boston Celtics, Dallas Mavericks, Denver Nuggets, Minnesota Timberwolves, and New York Knicks) for which search terms appeared in the Jan - Jun (YTD) 2024 search data.
<b>
5.  team_weekly_stats.csv

    Description - </b> This file contains the output of import_weekly_records.ipynb, the weekly and season-to-date winning-percentage numbers, by week (ending Sunday), for the NBA teams in the Google search data
<b>
6.  NBA Playoff records.csv 

    Description - </b> This file contains the date, teams, and results for every 2024 NBA playoff game through June, 2024 (incomplete results for NBA Finals between Boston and Dallas)
<b>
7.  teams_playoffs.csv 

    Description - </b> This file contains the merged playoff results and regular-season data to form a complete picture of 2024 NBA performance for the five teams searched in the Google data
<b>
8.  NBA 23-24 Records by Team, by Month - Merge Candidate.csv 

    Description - </b> This file contains data sourced from basketball-reference.com with the monthly records for all 30 NBA teams initially.
<b>
9.  NBA 23-24 Records by Team, by Month - Merge Candidate.csv 

    Description - </b> This file contains data sourced from basketball-reference.com with the monthly records for all 30 NBA teams initially.
    <b>
10. NBA 23-24 Records by Team, by Month - Merge Candidate.csv 

    Description - </b> This file contains another version of the  monthly records for all 30 NBA teams (beg. Jan. 2024) sourced from basketball-reference.com with the.
    

**#Title: Google Top 10 Big Query Search Terms**


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


