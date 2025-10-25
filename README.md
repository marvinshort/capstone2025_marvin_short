## Power Imbalance: Analyzing State-Level Electricity Generation and Consumption Disparities in the U.S.





#### Capstone Power BI Dashboard



Link: Power Imbalance: Analyzing State-Level Electricity Generation and Consumption Disparities in the U.S.





#### Motivation



My first professional job after graduating from college was with a company called [Asea Brown Boveri (ABB)](www.abb.com). They are a Global Top 100 Manufacturing company, headquartered in Switzerland, with a long history in manufacturing equipment that generates, transmits, or distributes power. This company hired me, an enthusiastic young college graduate who majored in Supply Chain Management, for their Supply Chain Management trainee program. I had the unique opportunity to work in 5 different factories across the United State. I supported production and delivery of substation transformers, low-voltage switchgear, automated power-switching relays, and heat recovery steam generators. Since then, the generation of power to meet mankind’s ever-increasing need for electricity has been a constant curiosity of mine. Also, my brother is an Electrical Engineer at the local utility company. 





#### Questions



* What resources does each state use to produce electricity? Is there any reliance on imports to meet needs?
* Which states have an electricity surplus or deficit? Does the surplus or deficit vary by month (season)? What percentage does each state contribute to the total US electricity output?
* Do these mismatches correlate with population size/density, presence of industries, climate, or geography?
* Are there any noticeable trends over time? Shift in resources mix, increase in electricity production efficiency?
* What are the factors driving the growth? (House building density, data centers, AI, and demand for electric vehicles)





#### Data Sources



* U.S. Energy Information Administration (U.S. EIA) - https://www.eia.gov
* U.S. EIA - Open Data Portal - https://www.eia.gov/opendata/ 
* U.S. EIA - Electricity Explained - https://www.eia.gov/energyexplained/electricity/how-electricity-is-generated.php

 





#### Technologies Used



1. Sublime Text (Build 4200) - for browsing extremely large (1.3 Gb) text file data dumps to identify data series to extract.
   
2. Anaconda Navigator 2.6.6/Jupyter Notebook 7.3.2/Python 3:

   (Pandas Module) - for exploration, formatting, filtering, slicing, and aggregation of the data

   (Requests Module) - for interacting with the U.S. Energy Information Administration API within a python notebook to query data from a website
   
3. Git - for backups and version control
   
4. Microsoft Power BI (v2.148.878.0, 64-bit) - for data visualization

   #### 

   

#### The Process



1. Gathered data from various sources.
2. Utilized python to cleanse the data.
3. Imported data into Power BI for visualization.
4. Summarize Insights

   

   

#### Problems and Hurdles



* You must register for an API key in order to access the data through an API.

  

* There was a learning curve to figure out how to make python interact directly with the API to retrieve data.

  

* The U.S. EIA API has a maximum record return limit of 5000 records per request so it took several request to build a complete data set.

  

* There were bulk data zip files available for download that contain large text files. These large files were too big for Python/Pandas to read and handle so other tools had to be installed. Sublime Text was installed to view the data and formatting within the text files. Dask was used to read in the text file line by line (without crashing the notebook), parse the data into manageable chunks, and then save individual chunks as separate CSV files. Python was then able to process each CSV file and merge them together.

#### 

#### 

#### Normalizing the Data



Since I was dealing with electricity data over time on both US and state level, the units of measure for different data sets were on different 	scales. US data was provided in Megawatt-hours (MWh) and state level data was provided both in Kilowatt-hours (KWh) and Thousand Kilowatt-hours 	(KWh). I had to convert the thousand Kilowatt-hours dataset to Kilowatt-hours (KWh) for analysis.





#### Conclusion

  

* Electricity generation and consumption is trending up year-over-year due to the ever-increasing computing needs of artificial intelligence, cloud-computing, electric vehicles, and e-commerce.



* There is a lot of ground still to be gained in electricity transmission and distribution efficiency.

  

* States that have a higher usage of renewable fuels have a headstart in becoming self-sufficient electricity producers.





#### Contact Me



* Email - [marvin.short@gmail.com](mailto:marvin.short+github@gmail.com)

  

* LinkedIn - [https://www.linkedin.com/in/marvin-short](https://www.linkedin.com/in/marvin-short)
