# Lyrics Generation

This code uses music from a provided Spotify playlist to generate new song lyrics.

## GetPlaylistScrapeLyrics.ipynb
This notebook first uses the Spotify API to get the name and artist for each song within a playlist.

Then, it scrapes lyrics for each song from [Genius](genius.com) and saves the entire corpus to a file, `playlist.txt`.

## NextWordPrediction.ipynb
This notebook adapts the idea of a next word prediction dictionary to generate lyrics for a song using the corpus generated in the previous notebook.

## Next Steps
- The next word prediction method employed above is fairly primitive, so using a more sophisticated method (LSTM is a common model for next word prediction) would probably lead to fewer strange results (as funny as they are!)
- Employing transfer learning — creating one model based on a corpus full of lyrics from different genres and time periods, then using the user supplied playlist to tweak the model — would improve performance especially, for shorter playlists.
