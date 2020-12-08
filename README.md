# LocalOBSTimer
A simple way to add customizable timers to OBS (Open Broadcast Software)

# Installation
Download the files to a folder on your stream computer

# Usage
* In OBS add a new web source.
* Set the Url to file:///C:\Your\Path\Here\counter.html?length=30
  DON'T SET LOCAL FILE CHECKMARK
* Set the width/height 
* Other options are by your preference
* Add the parameters to the URL according to your needs

# Parameters
* length - the number of minutes to count down
* startAt - the time (24h) to count down to. If the time is before the current time, count to the time tomorrow. If length and startAt are set, startAt wins.
* size - the font size
    sets the css fontsize so can use px, em, etc.
* color - the color of the counter
    sets the css color so can use named colors
* font - the font to use
    can specify any font installed locally on the machine
* align - the alignment
    choose left, center, right. Use center to auto center your source text but keep in mind fonts will cause the : to jump left/right by a few pixels during the count. Use Left to manually center your source text in OBS but not have the time : jump.


# Examples
countdown.html?length=3&size=255px&color=cornsilk&font=arial

countdown.html?startAt=10:30&align=left
