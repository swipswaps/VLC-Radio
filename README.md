# VLC-Radio Python script
Built for Python 3.6

install with 
```pip install VLCtagExporter ```

and run with 
``` python -m VLCtagExporter ```

Change the image and text file save directories. 
![locations](https://user-images.githubusercontent.com/27025504/34912780-43265264-f89e-11e7-9595-0ec692dd8e68.png)

# Requirements
The following python packages need to be installed, you can install them using these commands:
``` pip install Image
    pip install requests ```


This is a python script I built for streaming music using VLC media player. This script will read metadata from VLC media player for the song's title, album, artist, year released, genre, and album artwork. The album art will be automatically resized, and copied to the location of a folder specified in the script whenever a new song is played.

To change where the album artwork is saved, change the 'dst' variable on line 6 of the file. To change where the text file of song info is save, change the 'save_path' variable on line 8 of the program.

You can see a working example here: https://www.youtube.com/watch?v=eTXGcsqmj3g I used OBS studio for broadcasting, and set it up to display the jpg titled art.jpg in a folder, as well as display the contents of a specific text file. The album art and text file are automatically updated when their contents are changed.

# VLC Setup
To setup VLC Media Player, you will need to enable an online connection. You can find instructions on how to do so in this post:
https://stackoverflow.com/questions/24178980/how-to-monitor-vlc-media-player-on-windows-7-using-python

If you follow this guide, you will set a password for your vlc web interface, in the python file make sure you enter that same password in the s.auth = ('', 'password') field
