# PlaylistMerge KNN cluster

Using the Spotify Web API, this code authenticates a user and require input of 2 playlists. It gathers features about songs in the playlists, then using 
KNN cluster and machine learning it will y_pred spotipy recommended playlsits. Playlist 1 is given a y value of 0, Playlists 2 a 1 and it will add all
songs that are in the value of (.4 to .6), being in the middle of both. Will automatically create the playlist on users spotify.

#written in Python using Google Colab
