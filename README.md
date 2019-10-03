# HCDS-A1-Data-Curation

## Goal
The goal of this assignment is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through August 30 2019. All analysis are performed in a single Jupyter notebook and all data, documentation, and code is published in a single GitHub repository.The purpose of the assignment is to demonstrate best practices for open scientific research in designing and implementing a project, and make it fully reproducible by others: from data collection to data analysis.For this assignment, we combine data about Wikipedia page traffic from two different Wikimedia REST API endpoints into a single dataset, perform some simple data processing steps on the data, and then analyze that data.

## API
Wikimedia REST API: Links:

https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts (includes counts from web spiders/crawlers as well)
https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews (does not include views from web spiders/crawlers)

## Data
The Wikipedia data was gathered from the Wikimedia REST API, Wikimedia Foundation, 2017. CC-BY-SA 3.0
(https://creativecommons.org/licenses/by-sa/3.0/)

## Final Data description
The Final data is stored in the csv file: en-wikipedia_traffic_200712-201908.csv
* year : the year data was collected
* month : the month data was collected
* pagecount_all_views: total count of views from the legacy pagecount api for desktop and mobile combined
* pagecount_desktop_views: total count of views from the legacy pagecount api for desktop 
* pagecount_mobile_views: total count of views from the legacy pagecount api for mobile 
* pageview_desktop_views: total count of views from the pageview api for desktop (does not include page spiders/crawlers) 
* pageview_mobile_views: total count of views from the pageview api for mobile (does not include page spiders/crawlers)
* pageview_all_views: total count of views from the pageview api for desktop and mobile combined (does not include page spiders/crawlers)

## To be noted
The data from the Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not. The final vizualization therefore, contains some noise.
