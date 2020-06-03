# YT-PHASE
## YouTube Progress Hide And Show Encapsulation

A short javascript bookmarklet for those who want to hide the YouTube progress bar and navigation tools but also for those who want ro keep it constantly visible!

- Removing this bar for a moment can be pretty conveniant to take some screenshots for exemple.
- Having it always showing when playing music on youtube can be hugely usefull. No need to move the mouse around to enjoy the new named timestamps with the playing song name!

### Installation
To install it, just create a new bookmark, name it however you want (but preferably YT-PHASE like me!) and paste the following code as the URL:

```javascript
javascript:(function(){var ytp_bar=document.getElementsByClassName("ytp-chrome-bottom");var ytp_bar_opacity=ytp_bar.item(0).style.opacity;if(ytp_bar_opacity=="" || ytp_bar_opacity==0){ytp_bar.item(0).style.opacity=1}else{ytp_bar.item(0).style.opacity=0}})();
```
Add this bookmark to your browser toolbar and you are ready to use it!  
Each click will make the bar appear or disappear according to its current state.

### Notes
- Be aware that the javascript is executed once when you click on the bookmarklet, when reloading or changing pages its effect will no longer be active.
- The javascript might be a bit crude, do not hesitate to suggest improvements.
 
 <br/>
 
*This project is licensed under the terms of the MIT license.*

