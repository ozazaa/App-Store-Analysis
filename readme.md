# Communicate Data Findings : App Store Analysis 
## by Omar Zazaa


## Dataset : App Store

### Introduction

> Nowadays, smartphones became a necessity in our daily lives. People are starting to depend more and more on their phones in various aspects in our lives. In the following notebook, I will analyze data that was collected up until 2017 that was scraped from iTunes Search API regarding the Application in the AppStore, which contains around 7,000 apps. I Found This Dataset on Kaggle.com, it was full of insightful overviewing the Appp Store Market, and which apps users likes according to their rating.
The Variable in the original Dataset are as following:

### Files in Folder:
- AppleStore.csv           [Original Dataset]
- master_AppleStore.csv    [Wrangled Dataset]

- exploration.ipynb        [Exploration Analysis Jupyter Notebook]
- exploration.html           [Exploration Analysis Jupyter Notebook in HTML Format]

- explanatory.ipynb        [Explanatory Jupyter Notebook]
- explanatory.html         [Explanatory Jupyter Notebook in HTML Format]
- presentation.slides.html [Explanatory Jupyter Slideshow in slides.html Format]

- readme.md
- output_toggle.tpl

#### appleStore.csv
1.	"id" : App ID
2.	"track_name": App Name
3.	"size_bytes": Size (in Bytes)
4.	"currency": Currency Type
5.	"price": Price amount
6.	"ratingcounttot": User Rating counts (for all version)
7.	"ratingcountver": User Rating counts (for current version)
8.	"user_rating" : Average User Rating value (for all version)
9.	"userratingver": Average User Rating value (for current version)
10.	"ver" : Latest version code
11.	"cont_rating": Content Rating
12.	"prime_genre": Primary Genre
13.	"sup_devices.num": Number of supporting devices
14.	"ipadSc_urls.num": Number of screenshots showed for display
15.	"lang.num": Number of supported languages
16.	"vpp_lic": Vpp Device Based Licensing Enabled

### Wranligng Process

#### After visually and programitclly assesing the dataset and according to my goal toward this analysis alot of columns were dropped becuase they were irrelative to my analysis, dropped columns were:

- "id" : App ID
- "currency": Currency Type
- "ver" : Latest version code
- "cont_rating": Content Rating
- "ipadSc_urls.num": Number of screenshots showed for display
- "vpp_lic": Vpp Device Based Licensing Enabled

#### After the wrangling process my data consists of 2 types of variables mainly:
- The Numeric values which are related to size, user rating for all version and user rating for the latest version, price, number of supported languages & number of supported devices
- The Categorical values which were the prime genre and the currency.

#### To help make my analysis easier i added some other columns:
- "Status" = Free or Paid
- "fav_tot" = All Favortie Apps according to user rating score * total number of downloads
- "fav_ver" = Current Favortie Apps according to user rating for current version * total number of downloads
- "revenue" = price * total number of downloads.
- "size_mg" = converting the size of apps columns from bytes to Mega Bytes.
- "broad_genre" = the genres in the App Store which had the most number apps developed in it.

#### All of the variables created helped me have a better insight of the dataset, which led into a better analaysis.



## Summary of Findings

### General Questions:

-   How many Free and Paid Apps are there on the App Store?
-	The All Time Best Apps
-	The Current Best Apps (regarding this dataset up until 2017)
-	The Apps with the most revenue
-	The Apps with the Largest Sizes
-	The Most Expensive Apps made till 2017
-	Which Categories had the most Apps?


### Detailed Questions:

-	Are Paid Apps worth the purchase, and does the size of the app affect the price?
-	In Which categories are paid apps better than free according to the user experience and rating?
-	In Popular Categories what’s the ratio between paid and Free Apps?
-	Is there any relationship between user rating and total number of downloads to the price? or any other variable.


#### Most Questions were answered in both the Exploration Notebook and the Explanatory Notebook, with visualizes showing the answers clearly to the viewer, to help him understand the App Store Market in more insightful approach. This Analysis can help developers and entrepreneurs on deciding various aspects related to how they want to position their App in the Market.


## Key Insights for Presentation

Most of my graphs from the Exploration are present in the Explanatory Slide Deck, i didn't really have to polish any graphs in the process of moving from Exploration to Explanatory phase, as an analyst I think my visuals need to be as polished as possible in the Explorations phase so i can deliver the information clearly to the viewer.