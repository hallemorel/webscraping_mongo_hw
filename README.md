# webscraping_mongo_hw

For this project I built a web application that scrapes various websites for data related to the Mission to Mars and displays the information in a single HTML page.

Part 1, Web Scraping:

-  Used Jupyter Notebook, BeautifulSoup, Pandas and Request/Splinter.

-  Scraped the Nasa Mars News Site website and collected the latest news title and paragraph text: https://mars.nasa.gov/news/?page=0&per_page=40&order=publish_date+desc%2Ccreated_at+desc&search=&category=19%2C165%2C184%2C204&blank_scope=Latest.

-  Visited the JPL Featured Space website to gather images and used splinter to navigate the site and find the image url for the current Featured Mars Image: https://www.jpl.nasa.gov/spaceimages/?search=&category=Mars.

-  Using the Mars Weather Twitter account I scraped the latest Mars weather tweet from the page:https://twitter.com/marswxreport?lang=en.

-  From the Mars Facts webpage, I used Pandas to scrape the table containing facts about the planet including Diameter, Mass, etc. Converted the data to an HTML table string: https://space-facts.com/mars/.

-  Using the USGS Astrogeology site I obtained high resolution images for each of Mar’s hemispheres: https://astrogeology.usgs.gov/search/results?q=hemisphere+enhanced&k1=target&v1=Mars.

Part 2, MongoDB and Flask Application:

-  I used MongoDb with Flask templating to create a new HTML page that displays the information and the URLs from above. 

-  The Jupyter notebook was converted into a Python script with a function called scrape and then routed to the Mongo database query. 

-  The HTML template file holds and displays all of the Mars data and images.
