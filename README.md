# Spotipyproject

# **What Makes a Song Popular?**

![iPhone 12, 12 Pro – 1](https://user-images.githubusercontent.com/91847452/149189842-909628f3-08ef-40c3-bc45-de3b0ff0ca8b.png)

Music is something that has an important part in all of our lives. When we listen to our favorite song, we feel good throughout our whole body, since dopamine is released. In fact, listening to music is important to our health. That’s why we, Alara Alanbay, Stephanie Dito, Rafi Ahmed, and Michelle Liu, wanted to conduct a data science investigation about popular music. What makes a song popular? 

## _**Motivation**_

Exploring what makes a song hit the top charts is a fascinating study that caught our eye, as the study is a great mix between data analysis, sociology, and art. We are interested in the possibility of predicting, using the popular streaming platform Spotify, if there exists a set pattern which makes a song climb up the music charts. We aim to study audio features, which we can pull from Spotify’s API, of top music of the last few years. Is there a pattern? Are some audio features directly connected to others? Is there a defining audio feature that is prominent in all top songs? Is there a collective music taste, or are all the top songs different? We hope to answer these questions. 


## _**Overview**_
Our project’s aim was to use Spotify’s API to obtain data on audio features of top songs in order to analyse what makes a song popular. Our data sample is the Global Top 25 songs of every November from the years 2018 to 2021. We used SpotifyCharts.com to obtain these songs.

Now, we want to familiarise you with the audio features we concentrated on. 

The features that we chose have to do with the mood and production properties of the song. We feel that these features (tempo, danceability, valence, energy, speechiness, loudness, and instrumentalness) really contribute to what attracts the average ear to top songs. 

The description of audio features we have used, which we got from Spotify For Developers’ website, as follows:

**Danceability**: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity.

**Energy**: Energy represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy.

**Instrumentalness**: Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. 

**Loudness**: Loudness describes how loud the track is.

**Speechiness**: Speechiness detects the presence of spoken words in a track. 

**Tempo**: The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration

**Valence**: Valence describes the musical positiveness conveyed by a track. 


# _**Examples**_

We want to show you some top songs, so you can get an idea how the audio features values manifests in a top song. 

## **Taki Taki (with Selena Gomez, Ozuna, and Cardi B)** _By DJ Snake_

![Taki taki album](https://user-images.githubusercontent.com/91945641/148683880-55de9461-db89-44cf-9cd4-e81e3ae32ba5.png)

https://user-images.githubusercontent.com/91945641/148683616-e575c3eb-3672-4e8b-8800-92a7fb4a7266.mp4


<img width="395" alt="Screen Shot 2022-01-13 at 10 22 18 AM" src="https://user-images.githubusercontent.com/91945641/149312173-ebe8d019-2d3c-4d50-acb5-290874680c7d.png">



## **Easy on Me** _By Adele_ 

![adele album](https://user-images.githubusercontent.com/91945641/148683866-a03af351-6d1e-4abc-a390-cc5b551bcbec.jpeg)

https://user-images.githubusercontent.com/91945641/148683640-040045ad-3522-4f05-b2ea-a2d7971c671c.mp4

<img width="395" alt="Screen Shot 2022-01-13 at 10 21 24 AM" src="https://user-images.githubusercontent.com/91945641/149312175-1b89eb61-c6e8-4dc4-ac83-a24ea9fa2298.png">


![WhatsApp Image 2021-12-04 at 10 28 24 AM (1)](https://user-images.githubusercontent.com/91945641/148684206-6d948b8d-70f6-48fc-be20-9fdabdc69ef3.jpeg)

![WhatsApp Image 2021-12-04 at 10 28 25 AM](https://user-images.githubusercontent.com/91945641/148684185-c7be63a3-fd2b-4398-bacf-3617e04b76bd.jpeg)

Note: the features listed in the radar charts are a measure between 0 and 1. 

## A Puzzle

Taki Taki is the number one hit in November of 2018, while Easy on Me is the number one hit in November of 2021. As we can notice with these audio features, the two hit songs are quite different. 

How are they different from a data analyst’s standpoint? “Taki Taki” has a high valence and “Easy on Me” has a lower valence. This shows that any level of valence could climb up the charts. 

Another key difference is the energy levels, as “Taki Taki” clearly has a higher energy standing. 

Also we see some sort of correlation with energy and danceability, which we wanted to explore further.

From these songs’ data, we notice an irrelevance of speechiness here. Adele has a very low speechability as opposed to a relatively higher speechability in DJ Snake’s song. But when you listen to the music, it seems like Adele is singing more, while “Taki Taki” seems more instrumental. Our objective for studying speechiness was to see if more or less singing was more desirable to the human ear. But, this analysis shows that speechability measures do not help to explain our objective, as Adele’s top song is characterized by her lyrics. 

The only answer to our initial question that can be drawn from this comparison is that Both songs have high danceability, so that might contribute to the popularity of a song. 

### More Examples

![WhatsApp Image 2021-12-04 at 10 28 24 AM (2)](https://user-images.githubusercontent.com/91945641/148684312-e8f53094-9f5c-4e63-95ae-32ae70ca7752.jpeg)
![WhatsApp Image 2021-12-04 at 10 28 25 AM (1)](https://user-images.githubusercontent.com/91945641/148689454-a1d97e7a-2ca7-4779-910a-dcf493bc3d61.jpeg)

The top song in November of 2019 is "Dance Monkey" by Tones and I and the top song in November 2020 is "positions" by Ariana Grande.



![WhatsApp Image 2022-01-06 at 5 55 51 PM](https://user-images.githubusercontent.com/91945641/149195551-a7d582b6-d1d4-4e06-8548-6025707dcd91.jpeg)
![WhatsApp Image 2022-01-06 at 5 55 51 PM (1)](https://user-images.githubusercontent.com/91945641/149195554-3e8e6179-4546-442e-95bf-d1ac47c2b958.jpeg)
![WhatsApp Image 2022-01-06 at 3 01 30 PM](https://user-images.githubusercontent.com/91945641/149195566-93e2a012-008c-4561-8c84-1cf650756a47.jpeg)
![WhatsApp Image 2021-12-06 at 11 29 11 PM](https://user-images.githubusercontent.com/91945641/149195576-542242d8-0e5e-4402-ba52-520048158767.jpeg)

# _**Data**_
Using SpotifyCharts as a reference, we turned to Spotify's web API, Spotipy. After we created a Spotify web developer account, we created an APP and obtained our Client ID and Client Secret. Moving onto audio feature analysis, we first need to retrieve each individual track’s URI. We used Spotipy’s search feature, requested an Oauth token, and then proceeded with individual track’s data. We inputted the track’s name under “Q”, “track” under “Type”, and Spotipy produced a long list of code. After copying a track’s URI, we utilised the audio feature search tool, and the API gave us a list of all the different audio features already analysed by Spotify. We recorded these values in an excel sheet, and repeated the steps with the other tracks. 

We gathered a total of 100 data points, 25 songs over 4 years worth of charts. We compiled the data points into a singular excel sheet.

# _**Methodology**_
After compiling our data into Excel sheets, we ran descriptive statistics utilising Excel’s features. We calculated the mean, medium, maximum & minimum values as well as standard deviation on the audio features we selected I.e. tempo, valence, danceability, energy, loudness & speechiness for 2018-21. 

By looking at the values, there is a story emerging. The mean, median and standard deviation of tempo, energy and valence increases steadily between 2018 and 2021. This means that your favourite top songs, on average, are more likely to exhibit musical positivity, upbeat rhythms and energy over the years. However, the range of values of these audio features of top songs also expands over the years.

Conversely, the descriptive statistical values for danceability and loudness decreases steadily between 2018 and 2021. This means that your favourite mainstream song is potentially less loud and dancelike and most top songs have similar range of lower danceability and loudness over the years. This contradicts the media article’s assumption that songs rise in danceability over the years. 

The next step would be to investigate whether there is any relationship between the audio features that increase or decrease respectively. To do so, we exported this excel sheet into Stata and R respectively for data analysis. 
	
In order to study the relationship between a track’s position and its audio features, we turned to Stata to use a Simple Linear Regression (SLR) model. Regressions are used to determine the relationship between 2 or more variables, and quantitatively analyse how one variable changes when the other changes. We want to understand whether certain values of audio features will place a track higher or lower on the list. When these values change, we want to see whether their placement changes as well. 

In order to study the relationships between audio features, we used multiple regression analysis(MLR). MLR allows us to test relationships between multiple independent variables and a single dependent variable. For instance, we can test the direction and strength of relationship between danceability (dependent) with tempo, energy, valence, loudness i.e. all audio features. And we did! We constructed multiple MLR relationships to define each audio feature as y and rest as x: this is get a full combination of every single relationship possible over 4 years. Many times multiple factors affect one variable linearly in real life even if they are correlated with each other: None can make a song with just a single audio feature. Testing relationships allow us to explore common themes and interesting threads of popular music.

# _**Results**_
As illustrated above, the top 2 songs of two different years have drastically different makeup of audio features. However, they share a similarity of high danceability. Upon discovering this, we examined whether we can predict a track’s placement on the top 25 by its audio features.

With the Simple Linear Regression approach, we estimate the following equation:


<img width="630" alt="Screenshot 2022-01-12 at 18 04 00" src="https://user-images.githubusercontent.com/92088621/149196699-d34068b1-e9ea-49d1-b9e2-9435a66ebcd9.png">

The track’s position is the dependent (y) variable, and danceability is the independent (x) variable. β0 is the constant, ie. what is the track’s position when danceability equals 0. For the purposes of our project, we disregard β0. β1 serves as the coefficient in front of danceability. In other words, when the danceability increases by 1 unit, by how much does a track shift up on the charts. Ei serves as the error term for our equation, accounting for any confounding factors or errors in our estimation. 

<img width="839" alt="Screenshot 2022-01-12 at 17 43 58" src="https://user-images.githubusercontent.com/92088621/149193693-03c26b38-f3e6-42ad-926e-aa29ac8b0515.png">

Table 1 shows the Simple Linear Regression with our main explanatory variable, danceability, on chart placement. We find that at an aggregate level, danceability has a negative relationship with a track’s chart placement. A one unit increase in danceability is estimated to shift a track up by 8 positions on the top charts(in this case, a lower number, for example 1 or 2, translates to a higher position). A higher danceability value is associated with a higher placement on the charts. However, this coefficient is not statistically significant, ie. the results are likely to occur by chance. We wanted to examine how the 4 different years contributed to this coefficient, thus we broke it down in the following columns. 

In column 2, if a 2018 song has a high danceability value, it is actually positively correlated with their position on the charts. However, this coefficient is not statistically significant. This relationship is also apparent in column 3 with 2019 tracks and 2019 positions.

In column 4, if a song has a high danceability value, it is negatively associated with their position on the charts. Its coefficient is statistically significant at the 5% level; the results are not easily explained by chance alone. The same relationship and same statistical significance applies in column 5 with 2021 tracks and positions. 

On one hand, we obtained 2 years with positive coefficients. On the other hand, we obtained 2 years with negative coefficients. This leads to our negative coefficient in column 1 with no statistical significance overall. 
We observed that the relationship between positions and audio features fluctuate within each year between positive and negative, large and small coefficients. We continued to conduct SLR with other audio features against positions, such as valence and energy, but found danceability to have the most statistically significant results. Consistent with our findings, music is abstract; what makes a song popular has multiple confounding factors.


