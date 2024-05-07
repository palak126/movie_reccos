# movie rating prediction using Machine Learning and Big Data Tools
dataset link: https://www.kaggle.com/datasets/alanvourch/tmdb-movies-daily-updates<br>
Columns: 'id',<br>
 'title',<br>
 'vote_average',<br>
 'vote_count',<br>
 'status',<br>
 'release_date',<br>
 'revenue',<br>
 'runtime',<br>
 'budget',<br>
 'imdb_id',<br>
 'original_language',<br>
 'original_title',<br>
 'overview',<br>
 'popularity',<br>
 'tagline',<br>
 'genres',<br>
 'production_companies',<br>
 'production_countries',<br>
 'spoken_languages',<br>
 'cast',<br>
 'director',<br>
 'director_of_photography',<br>
 'writers',<br>
 'producers',<br>
 'music_composer'<br>

Schema of updated df <br>
root<br>
 |-- id: string (nullable = true)<br>
 |-- title: string (nullable = true)<br>
 |-- vote_average: string (nullable = true)<br>
 |-- vote_count: string (nullable = true)<br>
 |-- status: string (nullable = true)<br>
 |-- release_date: string (nullable = true)<br>
 |-- revenue: string (nullable = true)<br>
 |-- runtime: string (nullable = true)<br>
 |-- budget: string (nullable = true)<br>
 |-- imdb_id: string (nullable = true)<br>
 |-- original_language: string (nullable = true)<br>
 |-- original_title: string (nullable = true)<br>
 |-- overview: string (nullable = true)<br>
 |-- popularity: string (nullable = true)<br>
 |-- genres: string (nullable = true)<br>
 |-- production_countries: string (nullable = true)<br>
 |-- spoken_languages: string (nullable = true)<br>
 |-- cast: string (nullable = true)<br>
 |-- director: string (nullable = true)<br>

Summary statistics of numerical_columns(count, mean, std. deviation, min., max.)<br>
### vote_average<br>
+-------+------------------+<br>
|summary|      vote_average|<br>
+-------+------------------+<br>
|  count|            930297|<br>
|   mean|2.2410018167626307|<br>
| stddev|3.1242573440650556|<br>
|    min|               0.0|<br>
|    max|            17.287|<br>
+-------+------------------+<br>

### budget<br>                                                                                
+-------+-----------------+<br>
|summary|           budget|<br>
+-------+-----------------+<br>
|  count|           930297|<br>
|   mean|322878.5736245468|<br>
| stddev|5121834.967314752|<br>
|    min|              0.0|<br>
|    max|      6.4565466E8|<br>
+-------+-----------------+<br>

### revenue<br>                                                                                
+-------+--------------------+<br>
|summary|             revenue|<br>
+-------+--------------------+<br>
|  count|              930297|<br>
|   mean|    808810.969344448|<br>
| stddev|1.8265463620730754E7|<br>
|    min|               -12.0|<br>
|    max|               3.0E9|<br>
+-------+--------------------+<br>

### runtime<br>
+-------+------------------+<br>
|summary|           runtime|<br>
+-------+------------------+<br>
|  count|            930297|<br>
|   mean|46.566369165975914|<br>
| stddev| 58.39949621896666|<br>
|    min|               0.0|<br>
|    max|           14400.0|<br>
+-------+------------------+<br>

**analyzing trend in vote average**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/0042bdb5-d304-4cbc-bac5-6f597309e5f0)

**top 20 most frequent languages**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/c7462697-2f7f-41ed-905f-1fc8d141fc23)

**top 10 most popular genres**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/bc537b83-355c-4957-86bf-3e75d126e586)

**top 10 most popular directors**
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/73218e62-880d-4a3a-9a67-01105afd3557)

**overview length distribution**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/c3e70377-d5e9-4580-9c7f-d3061366023a)

**correlation matrix**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/5d9ebaae-2752-4d78-98c9-fb26f17795e5)

**buget vs revenue**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/a26ab5e2-6a00-400f-8b93-ed5a5d716d85)

**buget vs revenue by original language**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/9b9de1ad-a33e-401a-8498-95dff71945ef)

**analyzing trend in umber of movies released every year**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/d20403ac-8361-4f9e-9dd4-d8973f4e3a33)

**analyzing trend in average revenue over the years**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/b12622b4-af74-42e9-bccc-bde1f041dc2e)

**wordcloud for showing most common words in overviews**<br>
<br>
![image](https://github.com/palak126/movie_reccos/assets/149436003/5121de45-e8c6-4de7-a578-2abb83562649)

### Machine learning for predicting vote_average
Train size: (278524, 3)
Test size: (69631, 3)

##### Logistic regression 
Accuracy: 0.5590182533641626

##### Decision Tree
Accuracy: 0.5590182533641626

##### Random Forest 
Accuracy: 0.5590182533641626
