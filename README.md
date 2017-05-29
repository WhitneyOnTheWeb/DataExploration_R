# DataExploration_R
## P4: Explore and Summarize Data

Data Exploration is included in the [HTML file here](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/VGChartzExploration.html). Since it is too large to be viewed directly through GitHub, I've uploaded it to [my website where it can be viewed](http://whitneyontheweb.com/portfolio/VGChartzExploration.html).

Python script was adapted from the reference: https://github.com/GregorUT/vgchartzScrape

vgsales.csv was scraped from the VGChartz.com charts for regional and global video games sales (by millions of units). 
This data was obtained on 5/22/2017 using a Python3 script, [vgchartz.py](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/vgchartz.py), and importing BeautifulSoup to parse out the HTML data.

After the dataset was scraped from the table on VGChartz website, it was then limited to the top 10,000
rows, and formatted using a dataframe before being output to CSV for use in R. 

#### Scraped Data

- **Name** *(factor)*; Title of the video game
- **Platform** *(factor)*; Console/Platform game was released on
- **Year** *(num)*; Year game was released
- **Genre** *(factor)*; Genre/Category of the game title
- **Publisher** *(factor)*; Publisher of the video game
- **NA_Sales** *(num)*; Sales in millions of units in North America
- **EU_Sales** *(num)*; Sales in millions of units in Europe
- **JP_Sales** *(num)*; Sales in millions of units in Europe
- **Other_Sales** *(num)*; Sales in millions of units in other regions of the globe
- **Global_Sales** *(num)*; Total sales in units globally

#### Columns generated in R

- **Decade** *(factor)*; Decade the game was released
- **Franchise** *(factor)*; Name of the franchise the game is from
- **Company_Name** *(factor)*; Company that built the game console the game was published on

### Files

- **[VGChartzExploration.html](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/VGChartzExploration.html)**; Report knitted from RMD file created during exploration
- **[VGChartzExplortation.rmd](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/VGChartzExplortation.rmd)**; RMD file used to conduct exploration and knit file
- **[vgsales.csv](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/vgsales.csv)**; flat file containing dataset scraped from VGChartz and explored
- **[vgsales.py](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/vgchartz.py)**; Python script used to scrape file
- **[VGCharts_AnalysisInR.ipnyb](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/VGCharts_AnalysisInR.ipny)**; Jupyter Notebook used to do the work in R before moving it to R Studio in Visual Studio
- **[vgsales_overview.txt](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/vgsales_overview.txt)**; text file containing information about the data set and how it was obtained
- **[references.txt](https://github.com/WhitneyOnTheWeb/DataExploration_R/blob/master/references.txt)**; references used during the exploration
