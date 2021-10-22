# Spotify-Song-Recommendations

## Introduction

I'm a great music enthusiast and I absolutely love Spotify! But sometimes I feel like the song recommendations I get are heavily influenced by their popularity which makes me feel like I miss out on some hidden gems that I might actually love. So I decided to make a custom playlist with my own predictions of songs that I might like and not rely on Spotify's Algorithm. Since I have an extensive and obsessive record of Streaming History, it made my job easier and more accurate.



## Data Used
- Two datasets: "StreamingHistory.csv" (my Spotify listening history) and "SpotifyFeatures.csv" (dataset with songs and song features)
- StreamingHistory.csv was obtained through Spotify with a json drop.
- SpotifyFeatures.csv was downloaded from kaggle.

### Instructions and useful links to obtain data
- [Spotify Streaming History](https://thenextweb.com/news/a-simple-guide-to-visualising-your-spotify-listening-data-badass-ly)
- Spotify features dataset is already avaliable in this repo, just download the 'data used.rar' and you will find it.
- If you want to use my Streaming history you will find that in the 'data used.rar' file as well.



## Prediction Variable
- Our prediction variable will be called "favorite" with 1 representing a well-liked song and 0 representing otherwise. But, what is a 'favorite' song? I decided to label songs with more than 35 listens as a favorite and those with less as not.

- Why 35? When I plotted the song counts on a histogram, there was a substantial drop in song frequencies after 35. These cutoff seemed like a perfect place to differentiate songs that I listen to casually and the ones I obsess over :)

I've evaluated three models; Logistic Regression, Decision Trees and Random Forests to make predictions. Out of these three, I've concluded that Decision Tree Model is more efficient. 

The recommendations are stored as a csv file of the same name.



## Creation of the playlist
- You will find the python script to create the spotify playlist based on the recommendations we obtained under the name 'Playlist.ipynb'. 
- Make sure to obtain your token and OUATH from spotify and use it in the script. You can find the instructions on how to obtain the token etc. [here](https://stackoverflow.com/questions/60659902/how-to-get-oauth-token-from-spotify)
- This will then create a playlist by the name 'Custom rec'!

Here's a sample:

[Playlist](Playlist_sample.jpeg)
