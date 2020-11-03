# StockX Web Scraper
A web scraper to get product info and sales prices from stockx

## Overview
StockX is turning into a popular destination for buying and selling streetwear. Due to its bid/ask system vs more traditional auctions like eBay, it's also turned into the go to location to get an idea of an items value. I thought it would be a good project to get sales prices and potentially do some analysis to better understand reselling behaviour.

## Requirements
Selenium  
Pandas  
BeautifulSoup  
I used Firefox and the Gecko driver with Selenium, but you can change this is you prefer to use something else  

## Approach
-Launch Firefox
-Login to StockX (create a credentials.py file with your username and password)  
-Search StockX and get the urls of all the products retrieved by the search  
-For each url, go to the product page and get the details and historic sales prices  
-The product details and sales information are returned as 2 seperate lists  
-The lists are then converted to dataframes and the url can be used as a joining key  

## Future Improvements
Better deal with pages not loading correctly (can happen occasionally).  
Include a currency selector function.  
Cleanup the data (Remove currency symbols, commas etc).  
Convert dates.

