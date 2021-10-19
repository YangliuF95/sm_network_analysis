# The bibliometric dataset of social media data-based research domain
To download relevant bibliographic information on the complete set of papers for network construction, we combined data from two large databases, Web of Science (WoS) and Microsoft Academic Graph (MAG). The total number of 11,951 papers, 29,458 authors, and 543,809 citation relationships, are retained in our analysis.

## WoS dataset
The WoS dataset is proprietary and cannot be shared due to the terms of use by Clarivate @2021. Here we show the search strings for retrieving the metadata from WoS:

| **Queries (TS refers to search in title, keywords, and abstract fields)** | **Number of Publications** |
|---------------------------------------|------------------------| 
| #1 TS=("social media data”)           | 987|
| #2 TS=("social media" OR "social network* site*" OR "online social network*" OR facebook OR twitter OR instagram OR blog OR microblog OR YouTube OR Flickr) AND TS=(tweet* OR hashtag* OR weblink* OR posting OR commenting OR "news feed" OR user profile OR geotag* OR Youtube video OR "digital data" OR "computational social" OR "digital social" or "social web data") NOT TS=(survey OR questionnaire OR interview) | 11377|
| #3 TS=( facebook OR twitter OR instagram OR blog OR microblog OR YouTube OR Flickr) AND TS=(dataset) |1659 |
|Combine all queries #1 OR #2 OR #3     | 12732|
(Date: 3/17/2020)

## MAG dataset
MAG dataset can be downloaded via an Azure blob storage account. The detailed instructions for setting an account to download the dataset are available on the official website, https://docs.microsoft.com/en-us/academic-services/graph/. 

## Data format and data preprocessing
Both metadata downloaded are text files, we use Pandas to convert txt to CSV and conduct pair-wise matching between the two datasets.  

## Network and node attributes
The networks and related node attributes (including disciplinary background, community detected, and year) are provided here as edgelists and CSV files. We thank Clarivate @2021 for approving our request to share the network and node attribute data.
