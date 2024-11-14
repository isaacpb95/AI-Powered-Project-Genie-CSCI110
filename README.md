Pseudocode

1.	Define Global Variables:
	• Create two empty lists, songTitles and songArtists, to store song information.

2.	Define Functions:

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

3.	Main Program Loop:
	•	Repeat until the user chooses to exit:
	•	Display the menu:

1. Add Song
2. Playlist
3. Search Song
4. Save Playlist
5. Load Playlist
0. Exit

	•	Prompt the user to enter a selection.
	•	If select is 1, call addSong().
	•	If select is 2, call displayPlaylist().
	•	If select is 3, call searchSong().
	•	If select is 4, call savePlaylist().
	•	If select is 5, call loadPlaylist().
	•	If select is 0, print “Goodbye.” and exit the loop.
	•	If select is anything else, print “Please try again.”
