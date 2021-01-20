# python-api-challenge
# Python API Homework - What's the Weather Like?

## Background

Whether financial, political, or social -- data's true power 
ability to answer questions definitively. So let's take what 
about Python requests, APIs, and JSON traversals to answer a 
question: "What's the weather like as we approach the equator

Now, we know what you may be thinking: _"Duh. It gets hotter.

But, if pressed, how would you **prove** it?

![Equator](Images/equatorsign.png)

### Before You Begin

1. Create a new repository for this project called `python-ap
**Do not add this homework to an existing repository**.

2. Clone the new repository to your computer.

3. Inside your local git repository, create a directory for b
Python Challenges. Use folder names corresponding to the chal
**WeatherPy**.

4. Inside the folder that you just created, add new files cal
ipynb` and `VacationPy.ipynb`. These will be the main scripts
analysis.

5. Push the above changes to GitHub.

## Part I - WeatherPy

In this example, you'll be creating a Python script to visual
of 500+ cities across the world of varying distance from the 
accomplish this, you'll be utilizing a [simple Python library
python.org/pypi/citipy), the [OpenWeatherMap API](https://ope
api), and a little common sense to create a representative mo
across world cities.

Your first requirement is to create a series of scatter plots
following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

After each plot add a sentence or too explaining what the cod
analyzing.

Your second requirement is to run linear regression on each r
this time separating them into Northern Hemisphere (greater t
degrees latitude) and Southern Hemisphere (less than 0 degree

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots explain what the linear regression i
as any relationships you notice and any other analysis you ma

Your final notebook must:

* Randomly select **at least** 500 unique (non-repeat) cities
latitude and longitude.
* Perform a weather check on each of the cities using a serie
API calls.
* Include a print log of each city as it's being processed wi
number and city name.
* Save a CSV of all retrieved data and a PNG image for each s

### Part II - VacationPy

Now let's use your skills in working with weather data to pla
vacations. Use jupyter-gmaps and the Google Places API for th
assignment.

* **Note:** Remember that any API usage beyond the $200 credi
to your personal account. You can set quotas and limits to yo
to be sure you can't be charged. Check out [Google Maps Platf
(https://developers.google.com/maps/billing/
gmp-billing#monitor-and-restrict-consumption) and [Manage you
(https://developers.google.com/maps/documentation/javascript/
usage-and-billing#set-caps) for more information.

* **Note:** if you having trouble displaying the maps try run
nbextension enable --py gmaps` in your environment and retry.

* Create a heat map that displays the humidity for every city
of the homework.

  ![heatmap](Images/heatmap.png)

* Narrow down the DataFrame to find your ideal weather condit

  * A max temperature lower than 80 degrees but higher than 7

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Drop any rows that don't contain all three conditions. Yo
the weather is ideal.

  * **Note:** Feel free to adjust to your specifications but 
the number of rows returned by your API requests to a reaso

* Using Google Places API to find the first hotel for each ci
5000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap with each pi
**Hotel Name**, **City**, and **Country**.

  ![hotel map](Images/hotel_map.png)

As final considerations:

* Create a new GitHub repository for this project called `API
the kebab-case). **Do not add to an existing repo**
* You must complete your analysis using a Jupyter notebook.
* You must use the Matplotlib or Pandas plotting libraries.
* For Part I, you must include a written description of three
trends based on the data.
* For Part II, you must include a screenshot of the heatmap y
include it in your submission.
* You must use proper labeling of your plots, including aspec
Titles (with date of analysis) and Axes Labels.
* For max intensity in the heat map, try setting it to the hi
found in the data set.

## Hints and Considerations

* The city data you generate is based on random coordinates a
different query times; as such, your outputs will not be an e
provided starter notebook.

* You may want to start this assignment by refreshing yoursel
[geographic coordinate system](http://desktop.arcgis.com/en/a
guide-books/map-projections/about-geographic-coordinate-syste

* Next, spend the requisite time necessary to study the OpenW
Based on your initial study, you should be able to answer  ba
about the API: Where do you request the API key? Which Weathe
particular will you need? What URL endpoints does it expect? 
structure does it respond with? Before you write a line of co
aiming to have a crystal clear understanding of your intended

* A starter code for Citipy has been provided. However, if yo
extra challenge, push yourself to learn how it works: [citipy
(https://pypi.python.org/pypi/citipy). Before you try to inco
library into your analysis, start by creating simple test cas
main script to confirm that you are using it correctly. Too o
introduced to a new library, students get bogged down by the 
errors -- spending hours investigating their entire code -- w
simple and focused test would have shown their basic utilizat
library was wrong from the start. Don't let this be you!

* Part of our expectation in this challenge is that you will 
thinking skills to understand how and why we're recommending 
What is Citipy for? Why would you use it in conjunction with 
OpenWeatherMap API? How would you do so?

* In building your script, pay attention to the cities you ar
query pool. Are you getting coverage of the full gamut of lat
longitudes? Or are you simply choosing 500 cities concentrate
of the world? Even if you were a geographic genius, simply ra
based on your human selection would create a biased dataset. 
how you should counter this. (Hint: Consider the full range o

* Once you have computed the linear regression for one chart,
be similar for all others. As a bonus, try to create a functi
create these charts based on different parameters.

* Remember that each coordinate will trigger a separate call 
API. If you're creating your own criteria to plan your vacati
the results in your DataFrame to 10 or fewer cities.

* Lastly, remember -- this is a challenging activity. Push yo
complete this task, then you can safely say that you've gaine
mastery of the core foundations of data analytics and it will
from here. Good luck!

* Ensure your repository has regular commits (i.e. 20+ commit
README.md file

### Copyright

Trilogy Education Services © 2019. All Rights Reserved.
