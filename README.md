<h1>Data-Visualisation </h1>
Marvel Movies and its box office collection. 

<b>Video Link :</b> https://youtu.be/R6cr0aMhGQA

<h2>Dataset </h2>
•	I have used the following link to fetch data
https://www.the-numbers.com/movies/franchise/Marvel-Cinematic-Universe#tab=summary
•	My next dataset is extracted manually opening each film and extracting the cast list for the particular movie
•	Other data set is taken from 
https://www.the-numbers.com/movies/franchise/Marvel-Cinematic-Universe#tab=acting
•	I have also taken IMDB rating from 
https://www.imdb.com/imdbpicks/MCU-movies-ranked-by-imdb/ls038472133/mediaviewer/rm1589293056
•	Finally for the movie logo’s, I individually googled it and cropped to the desired pixel size

<h3>DATA CLEANING: </h3>
•	Ms Excel
•	Open Refine
•	Python
Data cleaning was primarily done using MS Excel.
I have used Open Refine to have consistent values in my dataset. In addition, one of fields was comma separated and I have extracted that into columns using Open Refine.
Python dataframe was used to perform aggregate operations for plotting data.

<h3>Interactive Line Chart with Dropdown options</h3>
My First graph is a line graph, which portrays Marvel Movie Collection in USD. X axis depicts the Date of Movie Release against Y axis depicting Amount in USD. The line graph projects 4 charts ie Production Budget, Worldwide Box Office Collection, Domestic Box Office Collection & Opening Box Office Collection, which is depicted by the legends. Dropdown options are provided which plots Worldwide Box Office Collection, Domestic Box Office Collection & Opening Box Office against Production Budget.
On Hover, the Movie Title with its respective Collection is visible. I have used datetime function to define X axis. Created 4 scatter plots and passed it into data. Then created a update menu bar which would toggle the 4 graphs depending on selection by basically hiding/showing the corresponding graphs. Used vibrant colors with Star markers to highlight points on each plot.


<b>Visualization created using: </b>
Plotly Using Python on Jupyter Notebook

<h3>Logarithmic Bubble Scatter Plot </h3>
Second Graph is a scatter plot with various attributes combined together. X-axis depicts celebrities’ worldwide box office collection and Y-axis represents his/her Franchise worldwide box office collection. The size of the circle represents the no. of appearances in a marvel movies whereas the different colors symbolize the % of Franchise/Career in earning ie Marvel’s impact on the celebrities total income. Due to big dataset for cast, I have used a logarithmic scale so that the points are distributed across the space. Every range is divided into traces with unique color and hover text info. Legends were not getting displayed properly due to plotly limitations. Color gradient is used with opacity increasing as we move from 90% to less than 10% of ratio of Franchise/Career. Manually assigned custom colors to each trace and calculated bubble size for plotting. Hover information displays the relevant information such as Celebrity Name ~ with his marvel character, No. of appearances, Franchise Collection vs Career Collection and the ratio between them.

<b>Visualization created using: </b>
Plotly Using Python on Jupyter Notebook

<h3>Bar chart with Line Plot</h3>
Third Graph is a Double axis graph, where X represents Movie Titles and left sided Y-axis represents the movie profit earned in USD and the other Y-axis represents the IMDB movie ratings. A simple box plot works wonder with line graph overlapped which shows the audience popularity of a movie through earnings against critic reviews for the same.
Simple color scheme has been used to represent bar graph with line graph. The Title names on the X axis have been slightly titled by an angle to fit the entire movie name.

<b>Visualization created using: </b>
Plotly using python on jupyter notebook

<h3>WordCloud</h3>
Finally an extra graph just out of curiosity for trying out visualization ie a simple online-generated word cloud depicting the no. of appearances of celebrities in marvel movies. A small tribute to Stan Lee for his wonderful studio.

<b>Visualization created using: </b>
WordCloud using https://www.jasondavies.com/wordcloud/

<h3>Result</h3>

Following are that factors I considered while doing the visualisation:
•	Use of multiple attributes in each graph to convey multiple information but cleanly and visually appealing with easy to understand.
•	Use of colors to depict attributes.
•	Proper labelling of Axes with Title info for every graph.
•	Deciding the Scale for each axes.
•	Providing dropdown where relevant.
•	Legends to be displayed appropriately.


Following are challenges faced:
•	Initially gathering the relevant dataset proved a challenge.  I had to manually combine dataset searching online to create a dataset, which I wanted for myself.
•	Tried my hands on various tools for visualization like Tableau, D3.js, Bokeh and finalized on plotly as it provided good visualization and had good support to fine tune various characteristics.
•	Major issue which I faced while plotting scatter plot was to display legend markers. Tried various options but could not get to display the legend markers due to plotly limitations as the legend markers are proportionate to the area of circle plotted. Finally changed the slope size to make it visible but still is not proportionate. 
•	Second setback I faced was working with images. I had gathered movie logos to be used for visualization (present in dataset). Tried multiple libraries to fit the datset. However, charts were not generated as planned with pixel issue or overlapping or size limitations. Failed to add images on hover or using images as bargraph plots.
•	I created word cloud using wordcloud library in python but was not very satisfied with the outcome, hence dropped the plan.
•	Also tried to create network-connected graph using D3.js and tableau for movie and cast list but faced technical difficulty in generating a meaningful graph, thus dropping those charts too.

