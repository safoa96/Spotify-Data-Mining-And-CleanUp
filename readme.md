## About the Project:-
Hello and welcome to my Spotify project! 🎶 We're here to explore the wonderful world of music, taking a close look at the most popular songs of 2022. My dataset, filled with information from Spotify, reveals everything you need to know about each track. I'll be covering things like the most popular music genres, the highest-ranked songs, danceability ratings, and more. Let's dive into the exciting realm of music together! 🎵

This project not only explores the depths of 2022's chart-toppers but also leverages Python application in web scrapping and the use of Spotify Web APIs. 

###### Wikipedia 
First I decided to carry out web scrapping (using BeautifulSoup) from the wikipedia page that contains the top streamed songs with specific attributes such as:
- **Rank**- Position a song is placed based on criteria such as highest streams
- **Artist** - Name of an artist of a song
- **Song** - Name of the song
- **Streams** - Total number of streams (measured in Billions)
- **Publish_date** - Date the song was released (provided in day, months, and year)

###### Spotify API
To obtain more data, I set up a developer account on the Spotify website to gain access to the Spotify API. To interact with the API, I utilized a Python library called Spotipy, which is designed specifically for the Spotify Web API. Spotipy is a simple and efficient tool that allows us to tap into the extensive music data offered by the Spotify platform.

To connect with the Spotify API, I obtained essential credentials, including the Client ID, from the developer dashboard. This involved creating a new application to acquire the necessary information for accessing the web API seamlessly..


![API-%20Dashboard.png](attachment:API-%20Dashboard.png)

You should get something like this as part of your credentials -

*Client ID = "85f2303ce08143ddbcf3470dcxxxxx"*

*Client secret = "1572c8ca77074fbcad0ad225dxxxxx"*

Through the API call, I successfully retrieved a variety of information. Among the wealth of data available, I carefully selected the most relevant details for my project. These include:

- **Artist**: Identifying the creator of the music. Data type - String
- **Followers**: Counting the number of people following a particular artist. Data type - Integer
- **Genres**: Categorizing the musical style or type. Data type - String
- **Artist Popularity**: Measuring the popularity of the artist. Data type - Integer
- **Song**: Identifying the specific track. Data type - String
- **Song Popularity**: Gauging the popularity of the song. Data type - Integer
- **Album Name**: Noting the name of the album containing the track. Data type - String
- **Album Release Date**: Capturing the date when the album was released. Data type - Integer

###### Extra Features

I also pulled in more data relevant to our project objectives;


- **Acousticness** - A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence; the track is acoustic. Data type - Float
- **Danceability** - Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable. Data type - Float
- **Energy** - Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy. Data type - Float
- **Instrumentalness** - Predicts whether a track contains no vocals. “Ooh” and “aah” sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly “vocal”. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0. Data type - Float
- **Liveness** - Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live. Data type - Float
- **Loudness** - The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typical range between -60 and 0 db. Data type - Float
- **Speechiness** - Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks. Data type - Float
- **Valence** - A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry) Data type - Float
- **Tempo** - The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration. Data type - Float

#### Dashboard :-

![newplot.png](attachment:newplot.png)

#### Url Links

Wikipedia: https://en.wikipedia.org/wiki/List_of_most-streamed_songs_on_Spotify

Spotify: https://open.spotify.com/playlist/0JiVp7Z0pYKI8diUV6HJyQ?si=24006a7dad1c4365#


## Challenge
Time constraints - There was some time constraint in putting togther this project as I had to change projects a number of times due to different challenges.
Cost - Many API versions required payment of huge sums before being able to use them.
Documentation Quality - I had to deal with the issue of inadequate and inconsistent data documentation which hindered our use and understanding of some APIs.
Limited Functionality - I found it challenging finding an API that provided us with the kind of data we were looking for.
Data Quality - Inconsistencies, inaccuracies and lots of null values in certain data sets.

## Limitations
Changes in API versions - This may affect API calls. It wiil be prudent to always read documentation to stay abreast with current API version.
Scope of Data- This data is limited to 2022. It will have to be enhanced to inlcude more years to gain more valuable insights.
