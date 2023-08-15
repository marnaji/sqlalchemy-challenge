# sqlalchemy-challenge
#### Climate analysis for long holiday vacation in Honolulu Hawaii.
I used Python and SQLAlchemy ORM to do the climate analysis and data exploration. The SurfsUp directory contains climate.ipynb Jupyter Notebook, the app.py Python script, and a Resources folder which contains the hawaii.sqlite database, hawaii_measurements.csv and hawaii_stations.csv.


#### Part1:
Analyze and Explore the Climate Data : 
I used provided files climate_starter.ipynb and hawaii.sqlite to start analyze and explore the data. 
to complete this section I used the SQLAlchemy create_engine() function to connect to the SQLite database.
then automap_base() function to reflect the tables into classes, and then save references to the classes named station and measurement. The app.py was created to design a climate app that includes the Flask API and 5 routes with JSON lists.

* ORM queries retrieves the data and prcp values related to the past 12 months. 
* Pandas has been use to create a DataFrame using the queried data. 
* used pandas to plot the results: 

<img src="/images/plot1.png" width="400" >
<img src="/images/plot2.png" width="400" >



#### Part2:
Design the Climate App: 
*I used Flask to create Climate API and 5 routes. 
1. `/`
* Start at the homepage.
* List all the available routes.

2. `/api/v1.0/precipitation`

* Convert the query results from your precipitation analysis (i.e. retrieve only the last 12 months of data) to a dictionary using date as the key and prcp as the value.
* Return the JSON representation of your dictionary.

3. `/api/v1.0/stations`
* Return a JSON list of stations from the dataset.

4. `/api/v1.0/tobs`
* Query the dates and temperature observations of the most-active station for the previous year of data.
* Return a JSON list of temperature observations for the previous year.

5. `/api/v1.0/<start> and /api/v1.0/<start>/<end>`
* Return a JSON list of the minimum temperature, the average temperature, and the maximum temperature for a specified start or start-end range.

For a specified start, calculate TMIN, TAVG, and TMAX for all the dates greater than or equal to the start date.

For a specified start date and end date, calculate TMIN, TAVG, and TMAX for the dates from the start date to the end date, inclusive.




### References
Menne, M.J., I. Durre, R.S. Vose, B.E. Gleason, and T.G. Houston, 2012: An overview of the Global Historical Climatology Network-Daily Database. Journal of Atmospheric and Oceanic Technology, 29, 897-910, https://journals.ametsoc.org/view/journals/atot/29/7/jtech-d-11-00103_1.xmlLinks to an external site.