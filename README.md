# YT-PHASE
## YouTube Progress Hide And Show Encapsulation

A short javascript bookmarklet code for those who want to hide the YouTube progress bar and navigation tools but also for those who want to keep it constantly visible!

- Removing this bar for a moment can be pretty conveniant to take some screenshots for exemple.
- Having it always showing when playing music on youtube can be hugely usefull. No need to move the mouse around to enjoy the new named timestamps with the playing song name!

### Installation
To install it, just create a new bookmark, name it however you want (but preferably YT-PHASE like me ! ) and paste the following code as the URL:

```javascript
javascript:(function(){var timer="";var player=document.querySelector('.html5-video-player');var ytp_bar=document.getElementsByClassName("ytp-chrome-bottom");var ytp_bar_opacity=ytp_bar.item(0).style.opacity;if(ytp_bar_opacity==""||ytp_bar_opacity==0){ytp_bar.item(0).style.opacity=1;player.showControls();document.getElementsByClassName("ytp-fullerscreen-edu-button")[0].style.opacity=0;timer=setInterval(function(){player.wakeUpControls()},1000)}else{ytp_bar.item(0).style.opacity=0;player.hideControls();document.getElementsByClassName("ytp-fullerscreen-edu-button")[0].style.opacity=0.9}})();
```
Add this bookmark to your browser toolbar and you are ready to use it!  
Each click will make the bar appear or disappear according to its current state.  
The timer progress bar and loading bar will update normally if shown.  
Also works on fullscreen mode!

### Notes
- Be aware that the javascript is executed once when you click on the bookmarklet, when reloading or changing pages its effect will no longer be active. At the moment, reloading is also the only way to get back the normal player behavior. The effect of the code seems to stay active when autoplay is enabled. Please share your experience with this functionnality.
- The javascript might be a bit crude, do not hesitate to suggest improvements. This code would not work properly if not used as a bookmarklet.
- This code has been tested and works on Chrome, Firefox and Brave, feel free to share your experience about other browsers.
 
 <br/>
 
*This project is licensed under the terms of the MIT license.*

