# PlaylistMerge KNN cluster

Using the Spotify Web API, this code authenticates a user and require input of 2 playlists. It gathers features about songs in the playlists, then using 
KNN cluster and machine learning it will y_pred spotipy recommended playlists. Playlist 1 is given a y value of 0, Playlists 2 a 1 and it will add all
songs that are in the value of (.4 to .6), hence being in the middle of both. Will automatically create the playlist on users spotify. Possibility of duplicates, might return to update and fix this issue.

Step 1 is using auth_manager=SpotifyOAuth, to sign in spotipy, then enter two playlist but hitting the 3 dots while inside of the playlist, then going to share > then "copy link to playlist" 

![Screen Shot 2022-07-18 at 4 53 44 PM](https://user-images.githubusercontent.com/107092609/179615485-c7e68a4b-5090-45aa-9b87-5fc0c5538dd7.png)

From there it's a bunch of data gathering from spotipy.audio_features then using those values and the contrast in values to train the data into fitting the rating of 0 or 1 from playlist 1 or 2. We then use sp.recommend to find songs based of random songs inside each playlist.

Using the trained KNN cluster algorithm we then y_pred on the recommended 
songs. The y_pred of middle values [.4,.6] will be added to the playlist

Finished product will show up in your playlists:

![Screen Shot 2022-07-18 at 4 51 22 PM 3](https://user-images.githubusercontent.com/107092609/179615190-0c056244-f16b-47d2-81da-6418e8498189.png)


Written in Python using Google Colab

