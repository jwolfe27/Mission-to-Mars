# Mission-to-Mars

## Purpose of Project
We built an application that scrapes data from multiple websites pertaining to Mars, and then displays all of the information gathered on a separate webpage.

## Scraping the Data:

### Scrape for Latest News Articles:
- Scrape data from 'https://data-class-mars.s3.amazonaws.com/Mars/index.html' to gather the latest news articles about Mars.
![Mars_Facts_Code](https://user-images.githubusercontent.com/89044350/139593137-a1707d4c-28fd-4793-b24e-94bba70c5654.PNG)

### Scrape for Mars Featured Image:
- Scrape data from 'https://data-class-jpl-space.s3.amazonaws.com/JPL_Space/index.html' to pull the latest "Featured Image" of Mars
![Mars_Featured_Image_Code](https://user-images.githubusercontent.com/89044350/139593223-f9c24590-5648-463d-b027-5d736607ea9f.PNG)

### Scrape for Mars Facts:
- Scrape data from 'https://data-class-mars-facts.s3.amazonaws.com/Mars_Facts/index.html' to pull the latest known facts about Mars
![Mars_Facts_Code](https://user-images.githubusercontent.com/89044350/139593280-6e1c0f67-9d22-48db-b2f9-a542b5d1ab06.PNG)

### Scrape for Mars Hemispheres Images:
- Scrape data from 'https://marshemispheres.com/' to pull the latest images the four hemispheres of Mars
![Mars_Hemispheres_Code](https://user-images.githubusercontent.com/89044350/139593330-cb8181af-106c-4a6b-97f8-5180a8dc8cc8.PNG)

## Applying MongoDB and Flask:
- Using MongoDB and Flask templating we create a new HTML page to display all of the data scraped from the above 4 URLs.
- After converting our .ipynb file to .py script we can use a "scrape" function that executes all of the code above and stores all of the data in a Python Dictionary.
- The index.html file takes the python dictionary data and displays it in HTML format.  Each time the "Scrape New Data" button is clicked, the information is fetched and updated in real time.
