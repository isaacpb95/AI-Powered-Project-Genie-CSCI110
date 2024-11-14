Define Functions:

Function addSong():
	•	Prompt the user to enter the song title and artist.
	•	Add the title to songTitles and the artist to songArtists.
	•	Print “Song added successfully.”

Function displayPlaylist():
	•	If songTitles is empty, print “The playlist is empty” and return.
	•	Otherwise, for each song in songTitles:
	•	Print the song’s index, title, and artist.

 Function searchSong():
	•	Prompt the user to enter the title of the song they want to search for.
	•	Set found to false.
	•	For each song in songTitles:
	•	If the title matches the search term:
	•	Print the song title and artist.
	•	Set found to true and break out of the loop.
	•	If found is still false, print “Song not found.”

Function savePlaylist():
	•	Open a file named “playlist.txt” for writing.
	•	For each song in songTitles:
	•	Write the title and artist to the file.
	•	Close the file.
	•	Print “Playlist saved to playlist.txt”.

Function loadPlaylist():
	•	Open the file “playlist.txt” for reading.
	•	If the file cannot be opened, print “File not found” and return.
	•	Clear both songTitles and songArtists lists.
	•	While there is more data to read in the file:
	•	Read a title and artist from the file.
	•	Add the title to songTitles and the artist to songArtists.
	•	Close the file.
	•	Print “Playlist loaded from playlist.txt”.

