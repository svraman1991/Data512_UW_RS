# Data512_UW_RS
Ramans repository for Data 512 Assignments - Au23

## Goal:
Understand basic data retrieval from Wiki pages and use the data to filter, combine and create new JSON datasets
Visualize trends from the data using python packages
Understand reproducibility and methods to use pre existing code or packages to create ones' own work

## Licenses:
The analysis here uses data from Wikipedia and its use is covered under - 
Wikimedia Terms of use: https://www.mediawiki.org/wiki/API:REST_API#Terms_and_conditions

Further, for the API's used, the documentation for their usage can be found at - 

Python requests module: https://pypi.org/project/requests/
Pageviews API: https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews

## Input file:
thank_the_academy.AUG.2023.csv.xlsx 
This is present in the root folder of this repo and it contains the list of films that were used for the analysis in this project

## Intermediate Data files:

As part of the code, CSV files of the data pulled were created, these are present under the CSV_Files folder: 
1) Desktop_Page_Views.csv
   
   a) This file has the output of the data pull for the desktop views of the movie list
   
2) Mobile_App_Page_Views.csv
 
   a) This file has the output of the data pull for the mobile app views of the movie list

3) Mobile_Web_Page_Views.csv
    
   a) This file has the output of the data pull for the mobile web views of the movie list

## Final Output files:
The final output is split across 2 folders: Pageviews and Images. Pageviews has the JSON file outputs for desktop and mobile and a cumulative view for the movies

Folder name: Pageviews
Files: 

1) academy_monthly_mobile_201501-202310.json
2) academy_monthly_desktop_201501-202310.json
3) academy_monthly_cumulative_201501-202310.json

Folder name: Images
This folder has the image output of 3 visual analyses performed as part of this project.
Files: 

1) avg_max_min
This graph is a time series representation for the articles with the highest average monthly page requests and the lowest average monthly page requests across both desktop and mobile interfaces.

2) top10_fewest
This graph is a time series representation of the top 10 article pages by peak page views across access type. 
The graph visualizes the top 10 items for desktop as well as the combined mobile access

3) top10_peaks 
This graph represents those movies that have the fewest months of available data for the most recent academy award winners.
The graph is a top 10 list of movies with the fewest months of data for both desktop and mobile access.

## Issues and considerations:

The data here is an analysis of mobile and desktop alone. 
Mobile data is a cumulative set of web and app access

The API pull can be modified to pull data corresponding to other access methods

The input file can be modified to include your own set of movies

The first code cell in python has a list of all libraries used as part of the code, executing this will let you know if you are missing any libraries and these can be installed via pip packages or Conda. 

