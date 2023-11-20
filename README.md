## McDonald's Google Reviews System

Dear reader,

I am Marc from the McDonald's data team and I am here to present you with the reviews scraping system I created.

This system consists on the scraping of google reviews of 8 of our restaurants here in Catalunya, as well as 5 other restaurants from out bigegest competitor, Burger King. 

My scraping system uses selenium to scrape the reviews from Google Maps, and therefore be able to, as a company, see what people have to say about their experience at our fast-food restaurants, as well as to compare what customers have to say about their visits to the BK franchise.

You will find 2 jupyter notebooks, an sql database and a tables folder with all the scraped restaurants.

### main.ipynb

Here is where the system runs. There are 2 functions:
- **Reviews**: extracts the google reviews from the inputted company and location (to try this, be sure to give a unique address for a unique restaurant, in order for Google Maps to identify the input as a valid company from where to extract its reviews.) The number of reviews to extract is at its optimal at 500 (my personal opinion), however, you will see it set as 100 due to the lack of time that I found when making the system, that is because, the extraction of 500 reviews can take up to 40 minutes. 

- **Information**: runs a rapid selenium on the same location and company inputed, where it aims to return a database with general information found on Google Maps of that location, that is: name of company, type of company, and address of company.

### tosql.ipynb

This jupyter notebook aims to join all the data extracted and send to MySQL to be able to perform the adequate queries.

### main.sql

This is the MySQL database of the my reviews system.

### Tableau Public

https://public.tableau.com/app/profile/marc.folch/viz/mcdoreviews/Story1?publish=yes

Sincerely, 

The McDonald's Data Team.

