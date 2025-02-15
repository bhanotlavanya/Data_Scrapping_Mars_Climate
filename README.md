# Data_Scrapping_Mars_Climate
This assignment consists of two technical products.

Scrape titles and preview text from Mars news articles.

Scrape and analyze Mars weather data, which exists in a table.

Part 1: Scraped Titles and Preview Text from Mars News
Used automated browsing to visit the Mars news siteLinks to an external site.. Inspected the page to identify which elements to scrape.

Created a Beautiful Soup object and used it to extract text elements from the website.

Extracted the titles and previewed text of the news articles that I scraped. Stored the scraping results in Python data structures as follows:

Stored each title-and-preview pair in a Python dictionary and, gave each dictionary two keys: title and preview. An example is the following:

{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
Stored all the dictionaries in a Python list.

Printed the list in notebook.


Part 2: Scraped and Analyzed Mars Weather Data
Used automated browsing to visit the Mars Temperature Data SiteLinks to an external site.. Inspected the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.


Assembled the scraped data into a Pandas DataFrame. The columns had the same headings as the table on the website. Here’s an explanation of the column headings:

id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location
Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.


Analyzed the dataset by using Pandas functions to answer the following questions:

How many months exist on Mars?
How many Martian (and not Earth) days worth of data exist in the scraped dataset?
What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
Find the average minimum daily temperature for all of the months.
Plot the results as a bar chart.
Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
Find the average daily atmospheric pressure of all the months.
Plot the results as a bar chart.
About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
Consider how many days elapse on Earth in the time that Mars circles the Sun once.
Visually estimate the result by plotting the daily minimum temperature.
Exported the DataFrame to a CSV file.