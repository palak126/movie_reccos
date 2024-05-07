# movie rating prediction using Machine Learning and Big Data Tools
dataset link: https://www.kaggle.com/datasets/alanvourch/tmdb-movies-daily-updates
Columns: 'id',
 'title',
 'vote_average',
 'vote_count',
 'status',
 'release_date',
 'revenue',
 'runtime',
 'budget',
 'imdb_id',
 'original_language',
 'original_title',
 'overview',
 'popularity',
 'tagline',
 'genres',
 'production_companies',
 'production_countries',
 'spoken_languages',
 'cast',
 'director',
 'director_of_photography',
 'writers',
 'producers',
 'music_composer'

Schema of updated df 
root
 |-- id: string (nullable = true)
 |-- title: string (nullable = true)
 |-- vote_average: string (nullable = true)
 |-- vote_count: string (nullable = true)
 |-- status: string (nullable = true)
 |-- release_date: string (nullable = true)
 |-- revenue: string (nullable = true)
 |-- runtime: string (nullable = true)
 |-- budget: string (nullable = true)
 |-- imdb_id: string (nullable = true)
 |-- original_language: string (nullable = true)
 |-- original_title: string (nullable = true)
 |-- overview: string (nullable = true)
 |-- popularity: string (nullable = true)
 |-- genres: string (nullable = true)
 |-- production_countries: string (nullable = true)
 |-- spoken_languages: string (nullable = true)
 |-- cast: string (nullable = true)
 |-- director: string (nullable = true)


+-------+------------------+
|summary|      vote_average|
+-------+------------------+
|  count|            930297|
|   mean|2.2410018167626307|
| stddev|3.1242573440650556|
|    min|               0.0|
|    max|            17.287|
+-------+------------------+
                                                                                
+-------+-----------------+
|summary|           budget|
+-------+-----------------+
|  count|           930297|
|   mean|322878.5736245468|
| stddev|5121834.967314752|
|    min|              0.0|
|    max|      6.4565466E8|
+-------+-----------------+
                                                                                
+-------+--------------------+
|summary|             revenue|
+-------+--------------------+
|  count|              930297|
|   mean|    808810.969344448|
| stddev|1.8265463620730754E7|
|    min|               -12.0|
|    max|               3.0E9|
+-------+--------------------+

+-------+------------------+
|summary|           runtime|
+-------+------------------+
|  count|            930297|
|   mean|46.566369165975914|
| stddev| 58.39949621896666|
|    min|               0.0|
|    max|           14400.0|
+-------+------------------+

![image](https://github.com/palak126/movie_reccos/assets/149436003/0042bdb5-d304-4cbc-bac5-6f597309e5f0)

![image](https://github.com/palak126/movie_reccos/assets/149436003/c7462697-2f7f-41ed-905f-1fc8d141fc23)

![image](https://github.com/palak126/movie_reccos/assets/149436003/c3e70377-d5e9-4580-9c7f-d3061366023a)

![image](https://github.com/palak126/movie_reccos/assets/149436003/5d9ebaae-2752-4d78-98c9-fb26f17795e5)

![image](https://github.com/palak126/movie_reccos/assets/149436003/9b9de1ad-a33e-401a-8498-95dff71945ef)

![image](https://github.com/palak126/movie_reccos/assets/149436003/d20403ac-8361-4f9e-9dd4-d8973f4e3a33)

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
