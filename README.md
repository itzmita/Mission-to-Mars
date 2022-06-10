# Mission-to-Mars
Learning web scraping

## Project Overview
The purpose of this project is to build a Web App that will scrape several websites for the most recent Mars data. The extracted data is stored in a NoSQL database and then an HTML page is created to display the findings.
In this project we learnt how to create a Web App which will scrape data from various website, in this case it will scrape the latest news and data related to Mars. Once the data is scraped we stored the details in a NoSQL Mongo DB. We also displayed the extracted details using HTML.

## Software
* Python 3.7
* splinter
* webdriver-manager
* Flask
* Flask-PyMongo
* BeautifulSoup (bs4)
* html5lib
* lxml

## Results

Scraping Mars Data
An example image of the HTML page created is shown below.


![image](https://user-images.githubusercontent.com/3753839/172985228-22570e50-9510-498a-b9c9-c51e6f8e744d.png)



Selecting the "Scrape New Data" button will obtain the latest news, images, and facts about Mars. This button invokes href="/scrape" which executes the following route in app.py

![image](https://user-images.githubusercontent.com/3753839/172985370-ff68405c-c076-425e-a900-1ebbc1335ada.png)




In the function scrape, we scrape the data using scrape_all function in scraping.py code to fetch the following details. 

![image](https://user-images.githubusercontent.com/3753839/172985377-50d1d609-2250-49cb-92fd-adbbaec84e71.png)



News titles and paragraph are fetched from 'https://redplanetscience.com'
The featured images are extracted from 'https://spaceimages-mars.com'
Facts about Mars are placed in a DataFrame from 'https://galaxyfacts-mars.com'. Here we learnt to use read_html to read a html data directly into a DataFrame.


### Deliverable 1 - Get the Hemisphere data with Image urls and titles
Hemisphere of Mars images are gathered from 'https://marshemispheres.com/'

![image](https://user-images.githubusercontent.com/3753839/172985834-86fec5be-fedc-46e3-ad48-7a75f21040ea.png)

### Deliverable 2 - Update the extracted data in Deliverable 1

After running app.py, the extracted data is successfully stored in MongoDB as seen in the screenshot below. 

![image](https://user-images.githubusercontent.com/3753839/172985430-c29087e3-715c-407f-8141-1315dcf6aa92.png)

### Deliverable 3 - Add Bootstrap3 components

Updating the index.html
Bootstrap 3 components were added such as the code below 
![image](https://user-images.githubusercontent.com/3753839/172985460-06710ec8-e2af-4d43-980e-78ec331e9c52.png)

which create this 
![image](https://user-images.githubusercontent.com/3753839/172985491-e423658f-369c-4b9b-beba-23a38d54a26f.png)

