interSubs
=========

Interactive subtitles for `mpv`, that was made to help study languages. Easily tweaked and customizable.

Uses http://pons.com/ for translation and http://linguee.com/ redirecting to browser by click.
Linguee, unlike Pons, bans excessive usage by IP, so don't overuse it or write scrapping functions for it.
Pons has an API, but it's limited to 1k requests per month, so scraping it is.

Can extend time of subs showing; for slow readers
    
    00:02:23,046 --> 00:02:25,990
    bla bla
    00:02:28,020 --> 00:02:33,084
    waka waka
    
    00:02:23,046 --> 00:02:28,020
    bla bla
    00:02:28,020 --> 00:02:33,084
    waka waka


![ezgif com-video-to-gif](https://cloud.githubusercontent.com/assets/10230453/22852882/683b508e-f04f-11e6-87d0-7477164a1709.gif)

Requirements
------------
   - Python 3
   - Lua
   - mpv (I don't know if it will work with mpv front-ends.)
   - optional: xdotool (for hiding subtitles when needed) 
   - optional: chromium (for external translation, other browser can be specified)
   - optional: wget (for listening to pronunciation)

Installation
------------
```
mv interSubs.py interSubs.lua ~/.config/mpv/scripts/
Edit configuration in interSubs.py
```
Usage
-----
- Start video with mpv & select subtitles.
- Press F5 to start/stop interSubs.
- Point cursor over the word to get popup with translation.
- Click on the word to look it up on another translator in your browser.
- Right-click on the word to hear its pronunciation, twice.
- Wheel resizes subtitles.
- Wheel+Shift changes its vertical position.
