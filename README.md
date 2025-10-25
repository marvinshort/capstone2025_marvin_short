# Power Imbalance:

## Analyzing State-Level Electricity Generation and Consumption Disparities in the U.S.





### Capstone Power BI Dashboard



**Link:** Power Imbalance: Analyzing State-Level Electricity Generation and Consumption Disparities in the U.S.





### Motivation



&nbsp;	From the very start of my career, energy and power systems have fascinated me. My first professional role was with [Asea Brown Boveri (ABB)](www.abb.com), a global leader in manufacturing equipment that powers the world. Fresh out of college with a degree in Supply Chain Management, I joined their management trainee program and had the privilege of working in five different factories across the United States. I supported the production and delivery of critical electrical components such as substation transformers, distribution transformers, power-switching relays, and heat recovery steam generators. That experience sparked a lasting curiosity about how we generate and distribute electricity to meet humanity’s growing demand. On a personal note, my brother works as an Electrical Engineer at our local utility company, which has only deepened my interest in this field. This capstone gave me the chance to explore that curiosity in depth and contribute meaningful insights into how electricity generation, transmission, and distribution need to evolve to meet future demands.





### Questions



* What resources does each state use to produce electricity? Is there any reliance on imports to meet needs?
* Which states have an electricity surplus or deficit? Does the surplus or deficit vary by month (season)? What percentage does each state contribute to the total US electricity output?
* Do these mismatches correlate with population size/density, presence of industries, or geography?
* Are there any noticeable trends over time? Shift in resources mix, increase in electricity production efficiency?
* What are the factors driving the growth in electricity need? (Population density, data centers, AI, and demand for electric vehicles)





### Data Sources



* U.S. Energy Information Administration (U.S. EIA) - https://www.eia.gov
* U.S. EIA - Open Data Portal - https://www.eia.gov/opendata/ 
* U.S. EIA - Electricity Explained - https://www.eia.gov/energyexplained/electricity/how-electricity-is-generated.php
* U.S. EIA - Electricity Losses - https://www.eia.gov/todayinenergy/detail.php?id=44436

 



### Technologies Used



1. Sublime Text (Build 4200) - for browsing extremely large (1.3 Gb) text file data dumps to identify data series to extract.
   
2. Anaconda Navigator 2.6.6/Jupyter Notebook 7.3.2/Python 3:

   (Pandas Module) - for exploration, formatting, filtering, slicing, and aggregation of the data

   (Requests Module) - for interacting with the U.S. Energy Information Administration API within a python notebook to query data from a website
   
3. Git - for backups and version control
   
4. Microsoft Power BI (v2.148.878.0, 64-bit) - for data visualization

   #### 

   

### The Process



1. Gathered data from various sources.
2. Utilized python to cleanse the data.
3. Imported data into Power BI for visualization.
4. Summarize Insights

   

   

### Problems and Hurdles



* In order to access some of the data from the U.S. Energy Information Administration (U.S. EIA), you must use their API. Registration is required to obtain an API key.

  

* There was a learning curve to figure out how to make python interact directly with the API to retrieve data.

  

* The U.S. EIA API has a maximum record return limit of 5000 records per request so it took several requests to build a complete data set.

  

* There were bulk data zip files available for download that contain large text files. These large files were too big for Python/Pandas to read and handle so other tools had to be utilized. I installed Sublime Text to view the data and formatting within the text files. I also had to install the Dask module in the python notebook. This module allowed me to read in the text file line by line (without crashing the notebook), parse the data into manageable chunks, and then save individual chunks as separate CSV files. Python was then able to import and process each CSV file and ultimately merge them together.

#### 

#### 

### Normalizing the Data



&nbsp;	Since I was dealing with electricity data over time on both US and state level, the units of measure for different data used different scales. US data was provided in Megawatt-hours (MWh) and state level data was provided both in Kilowatt-hours (KWh) and Thousand Kilowatt-hours (KWh). I had to convert the thousand Kilowatt-hours dataset to Kilowatt-hours (KWh) for apples-to-apples comparison.





### Conclusion



&nbsp;	Electricity generation and consumption is trending up year-over-year. Population growth, urban sprawl, industrial production, the need for more data centers (to support artificial intelligence and cloud-computing), and electric vehicle popularity are just a few of the many contributing factors.



&nbsp;	There is significant room for improvement in the area of electricity loss during generation (60%) and transmission \& distribution (5%).



&nbsp;	 Fuels used for electricity generation have different cost, availability, and electricity conversion efficiency associated with them. Some states (TN and NC) have adopted the strategy of using a balanced mix of fuels for electricity generation to mitigate risk. Other states (PA and VT) adopted the strategy of using mostly renewable energy sources that never exhaust.



&nbsp;	The United States electric grid must continue to evolve through a combination of sustainable practices and innovative technologies to meet future energy needs responsibly.





### Contact Me



* Email - [marvin.short@gmail.com](mailto:marvin.short+github@gmail.com)

  

* LinkedIn - [https://www.linkedin.com/in/marvin-short](https://www.linkedin.com/in/marvin-short)
