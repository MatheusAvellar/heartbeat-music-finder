# Heartbeat Music Finder
Find music that syncs with your heart rate!

This project is a proof-of-concept for a music finder that utilizes your heart rate to lookup music with the same BPM.

Ideally, users would have a more reliable way of getting their heart rate rather than feeling and clicking. Oh, well.

Here's the [live demo](https://matheusavellar.github.io/heartbeat-music-finder/index.html). However, I would advise against
multiple uses in short amount of times as this project is coded to fetch a webpage and then extract the BPM data from the
raw HTML. This is far from ideal and, considering the website is not an API endpoint, there's no telling how the server will
handle too many requests. The website in question is https://www.cs.ubc.ca/~davet/music/, made by
[Dave Tompkins](https://github.com/dtompkins). Reiterating, this is merely a proof-of-concept, and not intended as a full
blown website.
