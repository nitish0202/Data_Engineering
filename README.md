# Data_Engineering
Data Engineering Projects 

Extract Phase-

Extract the data from different sources. 
As a first step, I scrape the happiness data from Wikipedia. That is pulling the full html data from the Wikipedia link(https://en.wikipedia.org/wiki/World_Happiness_Report#2022_World_Happiness_Report) and then using BeautifulSoup to get the happiness table from the fetched html data

Next step, the population data for each country is fetched using API(https://rapidapi.com/aldair.sr99/api/world-population/) from Rapid API.

The average age per country is loaded by scraping the world data website(https://www.worlddata.info/average-age.php) similar to first step.

Tranform Phase-

Add a GDP column that can be computed by multiplying the columns “GDP per capita” and “Population”. 
convert the column “Population under 20 years old” to float by removing the percentage sign and converting the string to a float.

Load Phase-
In the load step, the final dataset is loaded into the expected format for storage. This could be a database, a CSV file or one of many other storage types. I stored this dataset in a CSV file
