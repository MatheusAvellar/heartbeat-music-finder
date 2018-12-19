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

The reason behind the use of Tompkins' website is simple: it is the only website I could find that has the possibility to
sort music by BPM. SoundCloud's API [also allows that](https://developers.soundcloud.com/docs/api/reference#tracks) and,
yes, that would be a perfect substitute, had they not disabled the registration of new apps.
<sup>[[1]](https://twitter.com/josephcohen/status/900359837963345920)
  [[2]](https://community.soundcloud.com/share-embed-230064/soundcloud-api-shutting-down-7381601)
  [[3]](https://docs.google.com/forms/d/e/1FAIpQLSfNxc82RJuzC0DnISat7n4H-G7IsPQIdaMpe202iiHZEoso9w/closedform)</sup>
Thus, in spite my searches, I eventually had to resort to using the botched filtering-html-with-regex method. Trust me, it
got ugly.

If you are interested, however, in how that RegEx works, I highly recommend using [RegExr](https://regexr.com/) with sample
HTML from the page.
