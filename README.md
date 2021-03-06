# MouseTrack

Track and display mouse movements/clicks over time. Old movements will get faded so it can be left running indefinitely.

This was made with the intention of recording mouse movements over multiple resolutions then merging them together. It is used by loading (and forgetting about) `main.py`, and using `generate_images.py` to create the images. All the calculations are done in a background process so that the tracking part shouldn't ever take a performance hit. Currently it only works on windows as it uses `win32api` to get all the information.

<b>Current Features</b>:
 - Track movement, clicks and key presses, over multiple resolutions
 - Display movement history ~~and click heatmap~~ (rewritten version coming shortly)
 - Fade out movement history to keep recent tracks more visible
 - Set colours of movement history
 - Keep separate tracks for different applications (a file called "Program List.txt" will be created with instructions)
 
<b>Known Issues:</b>
 - They keyboard stops being properly detected during full screen games.
 
<b>Example Output:</b>
<img src="http://i.imgur.com/rsugV3F.jpg">

<img src="http://i.imgur.com/XuEY8yg.jpg">
