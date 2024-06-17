# <center>ucb-data-analytics-project1-group5</center>
# Team Members

- <b>Iosif Vardoev
- Kayla Vaccaro
- Krutika Desai
- Scott Johnson
- Thay Chansy</b>
> Group Project Test

# Project1 Repository Files
 > <b>CODE FILES (.ipynb) 
1. exploratory_data_analysis_google.ipynb
 
    Description - </b> This file 
<b>
2. google_bi_query_lt_lg.ipynb
 
    Description - </b> This file 
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
2. Google_Bigquery_Top_Search_Jan_Jun_2024.csv
 
    Description - </b> This file contains the weekly search data, by DMA for the top-25 search terms in the United States on Google.com 
<b>
3. searched_teams_results.csv
 
    Description - </b> This file contains the regular-season Win/Loss records for the five teams NBA teams (Boston Celtics, Dallas Mavericks, Denver Nuggets, Minnesota Timberwolves, and New York Knicks) for which search terms appeared in the Jan - Jun (YTD) 2024 search data.
<b>
4.  team_weekly_stats.csv

    Description - </b> This file contains the output of import_weekly_records.ipynb, the weekly and season-to-date winning-percentage numbers, by week (ending Sunday), for the NBA teams in the Google search data
<b>
5.  NBA Playoff records.csv 

    Description - </b> This file contains the date, teams, and results for every 2024 NBA playoff game through June, 2024 (incomplete results for NBA Finals between Boston and Dallas)
<b>
6.  teams_playoffs.csv 

    Description - </b> This file contains the merged playoff results and regular-season data to form a complete picture of 2024 NBA performance for the five teams searched in the Google data





