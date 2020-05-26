# Now Clocking

Now Clocking is a Conky widget which shows a Monstercat style Now Playing when music is played via Spotify or cmus, or a clock when no music is playing.

I modified to be able to work in ArcoLinux and changed the configuration to adapt it to the modern conky config requirements.

It is working in ArcoLinux for me.

Other conkies I modified will be soon also accessible. If you are very impatient, you can follow my tutorial at YouTube: https://youtu.be/1uHQ1493c04 

![screenshot](https://imgur.com/kKjrMqz)

![screenshot 2](http://i.imgur.com/nAyLBTlm.png) ![screenshot 3](http://i.imgur.com/mshrZQUm.png) ![screenshot 4](http://i.imgur.com/Eglo1aim.png)

Imgur album containing full res images can be found [here](http://imgur.com/a/9Zcqu).

Please keep in mind that this widget was originally created for personal use only (and also I'm still new to this ricing thing) so the script used might be a little bit messy and inefficient. The Conky widget is even based on [Helix Conky](http://figman.deviantart.com/art/Helix-Conky-204016625) which has been heavily modified to make it look like how I want to.

## Dependencies

- [Spotify](https://www.spotify.com/)
- [cmus](https://cmus.github.io/)
- [ffmpeg](https://www.ffmpeg.org/)
- [dbus](https://www.freedesktop.org/wiki/Software/dbus/)

## Installation

1. Install the fonts "Gotham Bold", "Gotham Book", and "Montserrat Light".
2. Copy all files into `~/.config/conky`
3. Put the Conky widget into your desktop.
4. You might want to adjust the positioning of the widget since as said above, this widget is originally created for personal use only so I just made it specifically for my screen size, etc.

## Some questions you might ask

**Why are there 2 Conky widgets?**  
Conky has this weird transparency issue where the album art becomes semi-transparent when the widget background is set to transparent. The album art only becomes opaque when the widget background is opaque (which of course looks really bad), so I figured out that using 2 widgets (one for the text, and another for the artwork) can solve the problem.

**Why separate the files used by each music player?**  
I have tried merging `cmusart` and `spotifyart` into one file, I have also tried using only one file for the artwork and the text file, but this causes a bug where the artwork always re-downloads itself every time. So I think it's better to just use 2 files (once again this was initially created for personal use only).
