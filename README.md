# nets150hw5

A implementation-based project that aims to finds the similarity between songs in an existing playlist. The chosen playlist is the Global Top 50.

## Technologies used
1. Spotify API
   - used to retrieve songs and their respective artist from a playlist based on a Spotify URI
2. Genius API
   - used to retrieve the lyrics of selected songs
3. Professor Swap's Vector Space Model
   - used to calculate the cosine similarity between each song in the playlist
  
## SetUp
1. Collect your Oauth Token from Spotfiy and add it to APITokens file under the webScraping package.

* Go to https://developer.spotify.com/dashboard and log into Spotify using the following credentials: 
<br />Spotify Credentials
<br />email: nets150hw5@gmail.com
<br />password: bfsanddfs
    
* Go to [Get Oauth], scroll to the bottom of the page and hit "Get Token". Paste the generated token in the spotifyToken variable in the APITokens file.

2. Collect your Client Access Token from Genius and add it to APITokens file under the webScraping package.

* Go to https://genius.com/api-clients. Click log in and "Sign in with Google". Log into Genius using the same credentials as before.
    
* Click on "Generate Access Token". Paste the generated token into the geniusToken variable in the APITokens file.

3. The Spotify URI of the Global Top 50 playlist has already been generated. Feel free to change to a different playlist (has to be public!) by swapping out the Spotify URI.

* To do so, go to your Spotify web app and into your desired playlist. Right click on the playlist title > Share > Copy Spotify URI

4) Run the `Main` File  

## Troubleshooting
* The Spotify Oauth token expires very quickly. If you come across a `HTTP Error: 401` this could
be caused by an expired token. So just refer back to step 1 in the setup and generate a new token! 



[Get Oauth]: <https://developer.spotify.com/console/post-playlists/>


