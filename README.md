# Hollywood Movies Visualizations and Recommender System

## Introduction
<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this project, I do some analysis, visualizations, and then create movie recommender system on imdb data. I do that because I want to know more about movies, especially Hollywood movies. Therefore, I do analysis and visualization on imdb data which is contain informations about movies, e.g. who is produced, when the movies release, rating movies, budget and income, etc. After that, I create movie recommender system, which is the system will recommend top 10 similar movies based on the movie that has been input by the user.
 <br></br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The data that used in this project is data imdb that contain 81k+ movies and 175k+ cast members scraped from IMDb, taken from Kaggle (source : https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset). After that, I do preprocessing data so that data more clean or proper to use. Then, I do analysis to get insight or information from data, and make data visualization so that the data can be easily understood. And the last, I create movie recommender system content – based which is sistem will give movies recommendation based on some information from the data (e.g. genre, description, producer, etc) which similar with the movie that has been input by the user.
</p>

## Data
<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Data has been scraped from the publicly available website https://www.imdb.com. All the movies with more than 100 votes have been scraped as of 01/01/2020.
 <br></br>
 
-	The movies dataset includes 85,855 movies with attributes such as movie description, average rating, number of votes, genre, etc.

-	The ratings dataset includes 85,855 rating details from demographic perspective.

-	The names dataset includes 297,705 cast members with personal attributes such as birth details, death details, height, spouses, children, etc.

-	The title principals dataset includes 835,513 cast members roles in movies with attributes such as IMDb title id, IMDb name id, order of importance in the movie, role, and characters played.

 <br></br>
 Check this link for details of the data : https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset 
</p>

## Summary (Analysis, Visualization and Recommender System)
<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; First thing that I do in this project is preprocessing data, starting from filtering movie which is only USA or Hollywood movies that I used in this project, convert all currencies in the data into dollars, etc. The following are pieces of preprocessed data.
</p>

<p align="center"> 
 <img src="images/preprocessed data (1).png" /> 
 <img src="images/preprocessed data (2).png" /> 
 <img src="images/preprocessed data (3).png" /> 
 <br></br>
 Preprocessed data
</p>

<br></br>
<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; After that I do some visualizations on the data. Here are some analysis and visualization that  I have done.
</p>

#### - Which decade has release most movies and highest average vote (rating) ?
<p align="center"> 
 <img src="images/movie counts release based on decade.png" /> 
 <br></br>
 Movie counts release based on decade
 <br></br>
 <img src="images/average vote (rating) movies based on decade.png" /> 
 <br></br>
 Average vote (rating) movies based on decade
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Based on pictures above, numbers of movies released by movies industries almost always increasing every decade. However on 1960s, movie industry has decrease in the number of movies released. Meanwhile, on 2010s is a decade the most release numbers of movies that is 9784 movies. Then, on 2020s numbers of movies still a little bit, because the data taken in 2020, so that we don’t know which movie will be release in the following year on 2020s.
<br></br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Meanwhile in the second picture, can be seen that 1920s, 1930s and 1940s has movies average vote (rating)  which is quite high compared to other decades. Not only that, movies average vote (rating) have decrease on every decade after 1940s, This is inversely proportional to the number of films that are always increasing every decade.
</p>
<br></br>
 
 #### -	Which movie genre has most release and highest average vote (rating) ?
<p align="center"> 
 <img src="images/word cloud genre data.png" /> 
 <br></br>
 Word cloud genre data
 <br></br>
 <img src="images/top 5 genres based on movie counts and average vote (rating).png" /> 
 <br></br>
 Top 5 genres based on movie counts and average vote (rating)
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Can be seen on pictues above, drama movies were the most released movies with 22.40% of the total films, followed by comedy movies around 15.27%, romance moveis around 7.85%, etc. Based on the average vote (rating), documentary movies is the movies with the highest rating that is 7.5, followed by film-noir movies  with a rating around 6.64, biography movies with a rating around 6.6, etc.
</p>
<br></br>
 
 #### -	Which production company has release most movies, highest average vote (rating) and highest total income ?
<p align="center"> 
 <img src="images/top 10 production companies based on movie counts.png" /> 
 <img src="images/top 10 production companies based on average vote (rating).png" /> 
 <br></br>
 Top 10 production companies based on movie counts and average vote (rating)
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Based on pictures above, Metro-Goldwyn-Mayer (MGM) is the production company that produces the most movies that is 1263 movies, followed by Warner Bros produces 1119 movies, Paramount Pictres with 802 movies, etc. Meanwhile, based on average vote (rating), Walt Disney Animation Studio has the highest average vote (rating)  that is 7.11, followed by Stanley Kramer Productions and DreamWorks Animation which has same the average vote (rating) that is 6.86, etc. Then, the following is top 10 production companies based on total income.
</p>
<br></br>
 
<p align="center"> 
 <img src="images/top 10 production companies based on total income.png" /> 
 <br></br>
 Top 10 production companies based on total income
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; From picture above, we can see that Warner Bros is the production company which has highest total income that is around $81,653.87 M, followed by Universal Pictures with total income around $77,369.07 M, Columbia Pictures with total income around $64,742.51 M.
</p>
 <br></br>
 
 #### -	Which director has direct most movies and highest average vote (rating) ?
<p align="center"> 
 <img src="images/top 10 directors based on movie counts.png" /> 
 <img src="images/top 10 directors based on average vote (rating).png" /> 
 <br></br>
 Top 10 directors based on movie counts and average vote (rating)
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; From pictures above, Michael Curtiz is a director who has directed the most movies that is 97 movies, followed by Lloyd Bacon and Lesley Selander who has directed 78 movies. Meanwhile based on average vote (rating), Christopher Nolan became the number one director because he has average vote (rating)  around 8.29 which is the highest compared to other directors (the comparisons are quite far). Followed by Quentin Tarantine and Peter Jackson with the difference average vote (rating) is almost the same that is 7.87 and 7.82, etc.
</p>
<br></br>

#### -	Which actor or actress has acted the most movies and highest average vote (rating)?
<p align="center"> 
 <img src="images/top 10 actors or actress based on movie counts.png" /> 
 <img src="images/top 10 actors or actress based on average vote (rating).png" /> 
 <br></br>
 Top 10 actors or actress based on movie counts and average vote (rating)
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Based on pictures above, Eric Roberts is the actor who has acted in the most movies that is 192 movies, followed by John Carradine with 154 movies, Henry O’Neil with 139 movies, etc. Meanwhile, based on average vote (rating), Charles Chaplin is in first place with a average vote (rating) of 7.58, followed by Anthony Daniel and Montgomery Clift with the difference average vote (rating) is almost the same that is 7.35 and 7.34, etc.
</p>
<br></br>

 
 ## Movies Recommender System Content-Based 

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this section, I create movie recommender system content-based, which is this system will recommend top 10 most similar movies based on the movie that has been input by the user. The data used in this system are 'original_title' as index and  'genre', 'director', 'actors' and  'description' as a features. Then, the first thing that I do is preprocessing  data or text, e.g. case folding, tokenizing, stemming, etc. After that, create new column that is ‘bunch_of_words’ that contains words taken from all features columns which used as content or data for the recommender system. Here are pieces of preprocessed data.
</p>

<p align="center"> 
 <img src="images/preprocessed data recommender system.png" /> 
 <br></br>
 Preprocessed data
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; After the data is preprocessed, convert the data or collection of text documents to a vector of term or token counts (CountVectorizer). Then, calculate the cosine similarity, cosine similarity is a metric used to measure how similar the documents are irrespective of their size. The following is pieces of cosine similarity data.
</p>
<br></br>

<p align="center"> 
 <img src="images/cosine similarity data.png" /> 
 <br></br>
 Cosine similarity data
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; After calculated cosine similarity ,  create the function that return 10 recommended or similar movies based on movie which has been input by user. Here are codes of movie recommendation function.
</p>
<br></br>

<p align="center"> 
 <img src="images/codes of movie recommendation function.png" /> 
 <br></br>
 Codes of movie recommendation function
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Can be seen on picture above, movies recommender function will search or match the data according to user input. After that, do sorting on cosine similary data or values (from largest (most similar) to smallest (least similar)) from the data (or movie) that has been input by the user. After sorting the data, the function will take top 10 data (movies) from cosine similarity data, and then return the results which is the movies title and year released.
</p>
<br></br>

<p align="center"> 
 <img src="images/results recommender system.png" /> 
 <br></br>
 Result recommender system
</p>

<p align = "justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Can be seen from picture above,  that is the test results from my movie recommender system. In this test,  I input the movie which is “The Dark Knight”, and then the system recommends top 10 most similar movies based on the movie that has been input by me that is Batman Begins (2005), The Dark Knight Rises (2012), Batman Returns (1992), etc.
</p>

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
For details you can check my code : [Hollywood Movies Visualization and Recommender System.ipynb](https://github.com/rifkyahmadsaputra/Hollywood-Movies-Visualization-and-Recommender-System/blob/master/Hollywood%20Movies%20Visualization%20and%20Recommender%20System.ipynb)
