
<h1><center><font color="red">Final Project</font></center></h1>

<h2><center><strong>Capstone Project - The Battle of Neighborhoods</strong></center></h2>

<h2><center><font color="green">Clustering Analysis and Segmentation For Identifying Best Tourist place in INDIA </font></center></h2>

<center><font color="blue" size="10"> Mysore and Agra</font></center>

<p><b> Introduction/Business Problem</b></p>

<p>Mysore and Agra are the famous places in the world. They are diverse in many ways. Both are multicultural as well as the financial hubs of their respective countries. We want to explore how much they are similar or dissimilar in aspects from a tourist point of view regarding food, accommodation, beautiful places, and many more.</p>

<p>Today Tourism is one of the pillars of the economy and the people most often visits those countries who are rich in heritage and developed enough from a foreign prospective, like friendly environment. Every city is unique in their own way and give something new. And now the information is so common regarding location of every place around the world on your fingertips which make it easier to explore. Therefore, tourists always eager to travel to different places on the basis of available information, and the comparison (the part of the information) between the two cities always assist to choose the specific places or according to their choice</p>

<h2>Data Description</h2>

<b>To solve the problem, we will need the following data:</b>

<ul>
<li>List of neighbourhoods in Mysore and Agra. This defines the scope of this project which is
confined to the city of Mysore and Agra</li>
<li>Latitude and longitude coordinates of those neighbourhoods. This is required in order to
plot the map and also to get the venue data.</li>
<li>Venue data, particularly data related to shopping malls. We will use this data to perform
clustering on the neighbourhoods.</li>
</ul>

<p>For this problem, we will get the services of Foursquare API to explore the data of two cities, in terms of their neighborhoods. The data also include the information about the places around each neighborhood like restaurants, hotels, coffee shops, parks, theaters, art galleries, museums and many more. We selected one Borough from each city to analyze their neighborhoods.  We will use machine learning technique, “Clustering” to segment the neighborhoods with similar objects on the basis of each neighborhood data. These objects will be given priority on the basis of food traffic (activity) in their respective neighborhoods. This will help to locate the tourist’s areas and hubs, and then we can judge the similarity or dissimilarity between two cities on that basis.</p>


<strong><p>Sources of data and methods to extract them</p></strong>

<p><font type="Times new Roman">This Wikipedia page <a href="https://en.wikipedia.org/wiki/Mysore"> https://en.wikipedia.org/wiki/Mysore </a> and <a href="https://en.wikipedia.org/wiki/Agra">https://en.wikipedia.org/wiki/Agra</a> contains a list of neighbourhoods of both cities. We will use web scraping techniques to extract the data from the Wikipedia page, with the help of Python requests and beautifulsoup packages. Then we will get the geographical coordinates of the neighbourhoods using Python Geocoder package which will give us the latitude and longitude coordinates of the neighbourhoods.
After that, we will use Foursquare API to get the venue data for those neighbourhoods. Foursquare has one of the largest database of 105+ million places and is used by over 125,000 developers.Foursquare API will provide many categories of the venue data, we are particularly interested in the Shopping Mall category and other tourist places near to both cities in order to help us to solve the business problem put forward. This is a project that will make use of many data science skills, from web scraping (Wikipedia), working with
API (Foursquare), data cleaning, data wrangling, to machine learning (K-means clustering) and map visualization (Folium). In the next section, we will present the Methodology section where we will discuss the steps taken in this project, the data analysis that we did and the machine learning technique that was used.</font></p>

<b><h2>Methodology</h2></b>

<p>As we have selected two cities Borough to explore their neighborhoods. The data exploration, analysis and visualization for both boroughs are done in the same way but separately.</p>

<b><h2>Exploration</h2></b>

<p>For palace case, we have extracted information mysore palace from Wikipedia page. Then we arrange the data according to our requirements. In the arrangement phase, which applied multiple steps including to identify neighborhoods which have same geographical coordinates at each borough and sorted against the concerned borough. For data verification and further exploration, we use Foursquare API to get the coordinates of Mysore city and explore its neighborhoods. The neighborhoods are further characterized as venues and venue categories.</p>
<p>For agra, we used a saved data file which is already explored through foursquare API in which we have extracted all the boroughs of agra and then sorted against the concerned borough. Then we explored the agra neighborhoods as venues and venue categories</p>
<p>Before Clustering and segmentation of two cities Mysore and Agra preprocess the data by eliminating missing values.</p>

<b><h2>Visualization</h2></b>

<p>In the beginning, we visualize the selected borough neighborhoods so that we can get an idea or confirmation regarding the coordinates of that Borough. The second time after clustered the neighborhoods, we visualize the clusters to name them. Assigning the names are very important because it can identify the areas or specific places in each cluster. Here folium is used for visualization.</p>

<h2><b>Analysis</b></h2>

</p>We analyze both boroughs neighborhoods through one hot encoding (giving ‘1’ if a venue category is there, and ‘0’ in case of venue category is not there). On the basis of one hot encoding, we calculate mean of the frequency of occurrence of each category and picked top ten venues on that basis for each neighborhood. It means the top venues are showing the foot traffic or the more visited places</p>

<h2><b>Results<b></h2>

<p>After clustering the data of the respective neighborhoods, both cities (Boroughs) have venues which can be explored and attract the Tourists. The neighborhoods are much similar in features like Theaters, opera houses, food places, clubs, museums, parks etc. As far as concern to dissimilarity, it differs in terms of some unique places like historical places and monuments</p>

 <h2><b>Observations and Recommendations</b></h2>

<p>When we compare the tourist places, we observe that the historical place is only situated in Agra and the Monument or landmark venue is in Mysore neighborhoods. Similarly, Airport facility, Sculpture garden and Boat or ferry services are also available in Agra while venues like Nightlife, Climbing gym and Museums are present in Mysore.
<p>As far as concern to recommendations, we recommend Agra for visit Taj Mahl Place  Neighborhoods will be considered first to visit. The tourists have an easily travelling access due to Airport facility, which not only saves time but also helps to save money. This saved money can be utilized to explore more, the attracting venues.</p>

<h2><b>conclusion</b></h2>

<p>The Agra and Mysore neighborhoods have more like similar venues. As we know that every place is unique in its own way, so that’s argument is present in both neighborhoods. The dissimilarity exists in terms of some different venues and facilities but not on a larger extent.</p>


```python

```



