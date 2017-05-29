# DataExploration_R
P4: Explore and Summarize Data


Since the HTML file is too large to be viewed directly through GitHub, I've uploaded it to [my website](http://whitneyontheweb.com/portfolio/VGChartzExploration.html)

vgsales.csv was scraped from the VGChartz.com charts for regional and global video games sales (by millions of units). 
This data was obtained on 5/22/2017 using a Python3 script, and importing BeautifulSoup to parse out the HTML data.

After the dataset was scraped from the table on VGChartz website, it was then limited to the top 10,000
rows, and formatted using a dataframe before being output to CSV for use in R. 


The dataset is structured as follows:

• Name (factor); Title of the video game
• Platform (factor); Console/Platform game was released on
• Year (num); Year game was released
• Genre (factor); Genre/Category of the game title
• Publisher (factor); Publisher of the video game
• NA_Sales (num); Sales in millions of units in North America
• EU_Sales (num); Sales in millions of units in Europe
• JP_Sales (num); Sales in millions of units in Europe
• Other_Sales (num); Sales in millions of units in other regions of the globe
• Global_Sales (num); Total sales in units globally


Columns to be generated:

• Decade (factor); Decade the game was released
• Franchise (factor); Name of the franchise the game is from
• Company_Name (factor); Company that built the game console the game was published on
