FOLDER GUIDE
============

assets/artists/
  One square image per artist (used both on the "choose artist" page
  and as the vinyl label / song circle art if a song doesn't have its
  own cover). Name them to match the ARTISTS array in index.html:
    the1975.jpg
    taylorswift.jpg
    theridleys.jpg
    cubesplaylist.jpg

assets/audio/
  One ~1 minute chorus clip (mp3) per song. Name them to match the
  "audio" path in each song object, e.g.:
    the1975-song1.mp3
    taylorswift-song1.mp3
    ridleys-bewithyou.mp3
    ridleys-song2.mp3
    cube-song1.mp3

TO ADD A SONG
  1. Drop the mp3 in assets/audio and (optionally) a cover in assets/artists
  2. Open index.html, find that artist's "songs: [...]" array
  3. Copy one of the existing { title, from, cover, audio, lyrics } blocks,
     paste it as a new entry, and edit the fields

TO ADD AN ARTIST
  1. Copy a whole artist { ... } block in the ARTISTS array
  2. Give it a new id, name, cover image, and its own songs list

TIP: keep mp3s under ~2-3MB (export at 128kbps) so it loads fast on
mobile data, and use square images (at least 500x500px) for covers.
