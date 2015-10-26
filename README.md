# How-many-movies-in-amazon
Data warehouse course project2

##Introduction
The raw data are from snap.stanford.edu ,It's a comment dataset in amazon video section. The total size is approximately 9GB with 250,000 product ids. However, we want to know the true number of the product as different id may point to the same product.

##Details
- get_id.py : Clean the raw dataset to get distincted id and generate a list with product id
- core.py : crawl all the movie name with the list of product id and save it to database
- crawler.sh : Simple shell script to crawl only the http header data from amazon(which already include the movie name,quite time saving).

##Dependences
curl,python-numpy,python-MySQLdb,mysql-server,socks5 proxy(alternative)

##Test Environment
Ubuntu LTS 14.04(64-bit)
