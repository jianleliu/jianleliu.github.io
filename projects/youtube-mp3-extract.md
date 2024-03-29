---
layout: project
type: project
image: img/youtube-mp3-extract/youtube.png
title: "Youtube mp3 downloader"
date: 2023
published: true
labels:
  - Python
summary: "Extracts .mp3 audio file from youtube video."
---
<img class="img-fluid col-8" width="500" src="../img/youtube-mp3-extract/youtube.png"> <br>
Credit: internet
## Incentive

Months ago, youtube was trying to crack down ad  blockers, causing many of my musics on youtube unplayable. So I wrote a 
script to download a couple of my favorite songs to play locally.

# Youtube MP3 Extract

This script extracts mp3 audio file from a youtube video. The length can be changed by editing `env.py`. Specifically, the `start_time` and `end_time` in seconds. 

## Instructions

1. **Edit env.py:**
   - Open the `env.py` file and customize the following parameters:
     - `url`: The url of the youtube video.
     - `start_time`: Start time, in seconds, of the video.
        - 0: Default value, start at the start of the video.
     - `end_time`: The end of the video, in seconds. 
        - -1: Default value, end of the video. 
     - `output_file`: The name of the output file. None or provide a string name in env.py.

## Dependencies Installation
  1. Install requirements.txt either globally or in a virtual environment:
     - globally: pip install -r requirements.txt
     - virtual environment: 
        1. python3 -m venv "Replace with a name with no double quotes"
        2. run source path/to/venv/bin/activate
        3. run path/to/venv/bin/python avif_to_png.py

## Possible features
1. Download videos:
   - Able to trim with a range from start to end seconds.
2. Download an entire playlist of audio/video:
    - Use youtube API or
    - Extract website url
        - Have to deal with dynamic loading(selenium? BS4? Requests?)
        - HTML parser for urls
3. Make it possible to download video and convert into other video formats.
<hr>
<a href="https://github.com/jianleliu/scripts/tree/main/youtube-mp3-extract">
  <img src="https://github.com/fluidicon.png" alt="GitHub" width="25">
  jianleliu/scripts/youtube-mp3-extract
</a>
