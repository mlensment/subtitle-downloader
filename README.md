# Subtitle Downloader

Tired of finding subtitles online? This script does it automatically.

## Setup
* Install ruby (tested on 2.1.1)
* `sudo wget https://raw.githubusercontent.com/mlensment/subtitle-downloader/master/sub -P /usr/local/bin && sudo chmod +x /usr/local/bin/sub`
* To upgrade to the newest version:
* `sudo rm /usr/local/bin/sub && sudo wget https://raw.githubusercontent.com/mlensment/subtitle-downloader/master/sub -P /usr/local/bin && sudo chmod +x /usr/local/bin/sub`

## Usage
* Download your favourite show (legally).
* Navigate to the directory where you downloaded the file to (with terminal) and copy the filename.
* `sub The.Big.Bang.Theory.S07E24.HDTV.x264-LOL.mp4`
* `vlc The.Big.Bang.Theory.S07E24.HDTV.x264-LOL.mp4`
* Enjoy!

Optionally you can run `sub The.Big.Bang.Theory.S07E24.HDTV.x264-LOL.mp4 -r`  
This starts VLC player automatically, but does not detach from terminal.

## Under the hood
* This script goes to www.podnapisi.net, finds subtitles for your specified media file.  
* Lists subtitles by download count.  
* Finds the most downloaded English subtitles (when they are not on the first page, this simple script does not work).  
* Navigates to the download page.  
* Downloads subtitles, extracts them and renames them accordingly to the specified media file so they can be picked up by VLC player.
