## \#Power Imbalance: Analyzing State-Level Electricity Generation and Consumption Disparities in the U.S.







#### \##Table of Contents



##### \*\[Capstone Power BI Dashboard](#capstone-power-bi-dashboard)

##### \*\[Motivation](#motivation)

##### \*\[Questions](#questions)

##### \*\[Data Sources](#data-sources)

##### \*\[Technologies Used](#technologies-used)

##### \*\[The Process](#the-process)

##### \*\[Problems and Hurdles](#problems-and-hurdles)

##### \*\[Normalizing the Data](#normalizing-the-data)

##### \*\[Conclusion](#conclusion)

##### \*\[Contact Me](#contact-me)



#### 

#### \##Capstone Power BI Dashboard



Link:













#### \##Motivation



My first professional job after graduating from college was with a company called Asea Brown Boveri (ABB). They are a Global Top 100 Manufacturing company, headquartered in Switzerland, with a long history in manufacturing equipment that generates, transmits, or distributes power. I had the unique opportunity to work in several factories that made substation transformers, low-voltage switchgear, automated power-switching relays, and heat recovery steam generators. Since then, the generation of power to meet mankind’s ever-increasing need for electricity has been a constant curiosity of mine.





#### \##Questions



###### \###Initial Questions



* What resources does each state use to produce electricity? Is there any reliance on imports to meet needs?
  
* Which states have an electricity surplus or deficit? Does the surplus or deficit vary by month (season)? What percentage does each state contribute to the total US electricity output?
  
* Do these mismatches correlate with population size/density, presence of industries, climate, or geography?
  
* Are there any noticeable trends over time? Shift in resources mix, increase in electricity production efficiency?





###### \###Guided Questions



* What are the current challenges facing the U.S. electricity sector?



* What is the future outlook of the U.S. electricity sector?



* What are the factors driving the growth? (House building density, AI computing needs, data centers, growth of robotics and automation in manufacturing, EV popularity) 







#### \##Data Sources





* U.S. Energy Information Administration (U.S. EIA) - https://www.eia.gov



* U.S. EIA - Open Data Portal - https://www.eia.gov/opendata/

&nbsp;	

* U.S. EIA - Electricity Explained - https://www.eia.gov/energyexplained/electricity/how-electricity-is-generated.php

&nbsp;	





#### \##Technologies Used



\*\*\*\*\*\*\*\*\*\*\*\*\*Let's write down the languages we used, the libraries and its versions. \*\*\*\*\*\*\*\*\*\*\*\*\*\*





1. Sublime Text (Build 4200) - for browsing extremely large (1.3 Gb) text file data dumps to identify data series to extract
   
2. Anaconda Navigator 2.6.6/Jupyter Notebook 7.3.2/Python 3:

   (Pandas Module) - for exploration, formatting, filtering, slicing, and aggregation of the data
   (Requests Module) - for interacting with an U.S. Energy Information Administration API within a python notebook to query data from a website
   
3. Git - for backups and version control
   
4. Microsoft Power BI (v2.148.878.0, 64-bit)  - for data visualization





#### \##The Process



1. Gather data from various sources
2. Cleanse the data
3. Import into Power BI for visualization
4. Summarize Insights





#### \##Problems and Hurdles



* You must register for an API key in order to access most of the state level data



* Learning curve to figure out how to make python interact directly with the API to retrieve data



* The U.S. EIA API has a maximum record return limit of 5000 records per request



* There are bulk data zip files available for download that contain large text files. These large files are too big for Python/Pandas to read and handle so other tools had to be installed. Sublime Text was installed to view the data and formatting within the text files. Dask was used to read in the text file line by line (without crashing the notebook), parse the data into manegeable chunks, and then save as a CSV.





#### \##Normalizing the Data









#### \##Conclusion





Electricity Generation









Electricity Transmission and Distribution











Electricity Consumption



•	Residential Sector

•	Commercial Sector

•	Industrial Sector

•	Transportation Sector

•	Electric Power Sector





#### \##Contact Me



[marvin.short@gmail.com](mailto:marvin.short+github@gmail.com) - Feel free to contact me here



