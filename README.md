# $\textcolor{red}{Data\ Visualization\ on\ Amazon\ Prime\ Movies\ and\ TV\ Shows}$

### $\textcolor{red}{Data\ Choosen}$ : Amazon Prime Movies and TV Shows
The dataset is available on Kaggle.
Kaggle: https://www.kaggle.com/datasets/dgoenrique/amazon-prime-movies-and-tv-shows

This dataset, which details the American movies and TV episodes that are currently accessible on Amazon Prime, was compiled from Just Watch in March 2023. It consists of two CSV files: "titles.csv" and "credits.csv". We have merged the data from these two CSV files and used them in our project.
* title.csv - The "titles.csv" file contains more than 10k titles with 15 columns. These columns include the title ID, name of the title, show type (movie or TV show), a brief description, release year, age certification, runtime (for TV shows, the length of the episode), genres, production countries, number of seasons (if it's a TV show), IMDB ID, IMDB score, IMDB votes, TMDB popularity, and TMDB score.
* credits.csv - Over 140k credits of actors and directors are included in the "credits.csv" file, which has five columns that include the person ID on Just Watch, the title ID on Just Watch, the actor or director's name, the character name, and the role (either ACTOR or DIRECTOR). This dataset offers insights into the different kinds of content that are available on Amazon Prime, including genre and runtime distributions, popular titles, and details on the producers—such as the actors and directors—who worked on the project.

### $\textcolor{red}{Reason\ for\ choosing\ Tableau}$
* Two CSV files, title.csv, and credit.csv, with roughly 10k and 140k records respectively, are part of the Amazon Prime dataset. When working with larger datasets in such situations, Tableau is frequently chosen over Bokeh.
* Because of Tableau's strong data management features, users can work more effectively and efficiently with massive datasets.
* Additionally, it provides a large variety of data connectors, making connecting to various data sources simpler.
* To quickly build new visualizations, Tableau provides a selection of pre-built templates, charts, and graphs. Analyzing a dataset and making fast prototypes can be helpful.
* When dealing with massive datasets like Amazon Prime, it is challenging to identify patterns and trends in the data without a suitable visualization.
* With Tableau's customization features, we have the power to effectively communicate the most important data points from the data set.

### $\textcolor{red}{Requirement\ Gathering\ and\ project\ planing\ using\ Mural\ Board}$
![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/cf5582c2-afb0-48ef-b436-cead934a0a0e)

### $\textcolor{red}{Potential\ Questions\ that\ are\ answered\ by\ analysis\ and\ visualization}$
![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/5961171e-f30d-4ea3-9b67-458f55991adb)

### $\textcolor{red}{Data\ Types\ and\ Interaction\ with\ Report}$

### $\textcolor{red}{Pre\ processing\ on\ the\ dataset}$
* The title.csv contains 10k records with 15 columns and credits.csv contains 140k records with 5 columns.
* Therefore, before creating the visualization, pre-processing should be done on such big datasets.
* Libraries used for preprocessing the data:
  -- ast - The Python library ast provides a way to parse and manipulate the source code of a Python program.
  -- MultiLabelBinarizer - The class is imported from sklearn.preprocessing module and is used to convert a list of labels 
     into a binary matrix representation, and is often used in multi-label classification tasks.
  -- pandas - The Python library pandas are used for reading, manipulating, and analyzing data.
  -- NumPy - NumPy is used while working with arrays and matrices of numerical data.

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/51753135-dbbe-4e98-9781-f6297cb6e763)

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/0a12da1a-87ba-48dd-a4e8-def4b3ec35f8)

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/10494bb9-9b97-48cc-ab8e-6e424be642d6)
![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/b1743736-0a73-4e0b-beb5-b6808e6aaa53)

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/a90653d8-7db3-4c32-96c5-25bc3efb0b1a)

### $\textcolor{red}{Dashboard\ Plots\ and\ respective\ Questions}$
#### $\textcolor{red}{1:\ What\ is\ the\ distribution\ of\ Content-Type\ Shows\ across\ genre\ and\ production\ countries?}$
The below plot is used to depict the distribution of the content type (movies and TV Shows) across the different genre grouping, release years, and production countries using a pie chart. We have used the multi-value drop-down filter for release year, genre grouping, and production countries. The distribution of the pie chart (size) will change based on the genre grouping, release year, and the country we select in the filter. 
* The pre-attentive attribute used is - color and size. 
* Color: Blue color represents the percentage of movies and green color represents the percentage of TV shows.

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/79bcafc7-8bfe-492f-938d-582cb5b2cb42)

#### $\textcolor{red}{2:\ What\ is\ the\ distribution\ of\ Titles\ by\ Type\ across\ genre,\ age\ certification,\ production\ countries,\ and\ release\ year?}$
The below plot is used to depict the distribution of the title across different genre groups, age certifications, and production countries using a line chart. We have used the multi-value drop-down filter for age certification, genre grouping, and production countries. Using the filter, we can select one or more combinations of inputs to get the desired distribution of titles.
* The pre-attentive attribute used is – position and color. 
* Color: Blue color represents movies and green color represents TV shows

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/0e306438-300a-40ae-ac92-e210903e0899)

#### $\textcolor{red}{3:\ What\ is\ the\ distribution\ of\ age\ certification\ across\ genre,\ priduction\ countries,\ and\ release\ year?}$
The below plot is used to depict the distribution of the age certification across different genre groups, release years, and production countries using a bar chart. We have used the multi-value drop-down filter for release year, genre grouping, and production countries. Using the filter, we can select one or more combinations of inputs to get the desired bar chart depicting the distribution of age certifications.
* The pre-attentive attribute used is – length and color. 
* Color: Blue color represents movies and green color represents TV shows

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/6a560103-d143-40db-9061-d73cdbdfe918)

#### $\textcolor{red}{4:\ What\ are\ the\ top\ N\ countries\ based\ on\ content\ production\ across\ age\ certification?}$
The below plot is used to show the top N countries based on content production across the age certification using a stacked bar chart. We have used the multi-value drop-down filter for the age certification and production countries, the multi-value list filter to select one or more content types, and the top N filter to select the required top n values to be displayed on the chart. Using the filter, we can select one or more combinations of inputs to get the desired bar chart depicting the top N countries based on content production across age certification.
* The pre-attentive attribute used is – length and color. 
* Color: Blue color represents movies and green color represents tv shows

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/f5df63ee-a057-443e-a122-345b51353ed7)

![image](https://github.com/swethamurthy25/Data-Analysis-Visualization-on-Amazon-Prime-Movies-TV-Shows/assets/112581595/6a560103-d143-40db-9061-d73cdbdfe918)
