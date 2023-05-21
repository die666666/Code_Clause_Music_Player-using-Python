# Music_Player-using-Python


The code imports necessary modules and libraries: tkinter for the GUI, fnmatch and os for file operations, and mixer from pygame for playing audio. The GUI window is created with the title "Music Player" and a size of 800x600 pixels. The background color is set to navy blue.The Pygame mixer is initialized to enable audio playback. Image files for previous, stop, play, pause, and next buttons are loaded using tk.PhotoImage.

Several functions are defined for different actions:

select(): function loads and plays the selected music file from the listbox.

stop(): function stops the currently playing music.

play_next(): function plays the next song in the listbox when the "Next" button is clicked.

play_prev(): function plays the previous song in the listbox when the "Prev" button is clicked.

pause_song(): function pauses or unpauses the currently playing music.

A Listbox widget is created to display the available music files. The selected filename is shown in a Label widget. Buttons for previous, stop, play, pause, and next actions are created and packed in a Frame widget. The code uses os.walk() and fnmatch.filter() to iterate over the files in the rootpath directory and add the filenames to the listbox.

Becareful while creating a rootpath it may cause error it can resolve: By adding an extra backslash or using a raw string, you avoid the Unicode error related to the backslash character.
