# Identifying the most crowded subway stations in New York city during Summer 2021
Nada Rambu

### Abstract
The goal of the project is to to identify the staions with the most traffic in the upcoming Summer using the Metropolitan Transportation Authority (MTA) turnstile data, which will help WomenTechWomenYes (WTWY) organization to distribute awareness by reaching out to a wider segment of people.
In order to explore the data, the data of Summer season (i.e., June, July, and August) in 2019 was uploaded to a PosetgresSQL database in an AWS cloud. After that, the datasets were preprocessed then plotted to extract and analyse some useful information that stasfies the goal.

### Design
WomenTechWomenYes (WTWY) is a fictional organization that aims to draw attention to their upcoming summer gala. Taking advantage of New York MTA turnstile data, the stations with the highest traffic can be recognized in order to determine the optimal placement for their street teams, allowing them to reach out to a wider segment of people who are interested. Luckily, the MTA is providing a [weekly data about their turnstile usage across New York city.](http://web.mta.info/developers/turnstile.html)

Assuming that the data has pattern in each season, the data of Summer 2019 will be explored for the purpose uncovering any underlying ridership patterns during Summer. (the data of 2020 was purposely ignored because of the pandamic impact on the patterns)

### Data
Each file of data contains more than 190000 row, where each row of the dataset represents a single entry or exist through a turnstile. Merging the data on one dataset resulted in a 5583045 row, with 11 categorical feature except for the ENTRIES and EXITS being integers type (the feature description can be found on their [official website (http://web.mta.info/developers/resources/nyct/turnstile/ts_Field_Description.txt) and 
one addtional aggregated feature that represent the date and time together as a timesamp. The dataset was also grouped by specific features in order calculate the maximum entries per turnstile and per station.

### Tools
AWS RDS to create a cloud
PostgreSQL for data storing
SQLAlchemy to load the data into Python
Numpy and Pandas for data manipulation
Matplotlib and Seaborn for plotting

### Communication
