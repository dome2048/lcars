These are template SVG files for use with openHAB's HABPanel interface. They are designed from a 2370's era Star Trek LCARS design aesthetic.

They are still very much a work in progress. I'm making them available now upon request.

While I may someday make them into a universally functional demo, they are currently optimized for my home and won't be useful to others without heavy modification.

The 3DIN is a tablet designed for my dining room. It's designed to be general purpose, with a display for security cameras, a map with a security overview, basic weather info, and scene shortcuts.

The other three are all located at the same desk location. Left and right sit on either side of my main computer setup. Left is set up as a system overview, with weather and a map. On the right is a frame based panel, which allows me to display cameras, logs, BasicUI, PaperUI, or any other web based application in a frame. The Panel version runs on a Raspberry Pi touchscreen and is designed to be the only one of the three that is frequently interacted with directly (as opposed to being optimized for viewing). It has several "pages" of controls that are shown or hidden based on a String item, and allows control of the right display (as explained above), direct device control, scene selections, audio control, and an alert condition section.

To make sense of the office panel SVG, I recommend hiding all of the control layers except the one you want to view. Otherwise it's unintelligible.

For fun, most elements respond to a change in the relevant Condition string item to display animations for Red Alert, Yellow Alert, and Blue Alert. I took some artistic license with exactly how the items were rendered. I noticed that in later shows, more and more of the elements would change colors to reflect the alert status and I thought that looked great, so I'm aiming to have as many elements react to the alerts as possible.

The files are created (and best viewed and edited with) Inkscape. I used Mac OS version 0.92.2. 

For use, I recommend compressing them using SVGO: https://jakearchibald.github.io/svgomg/ Disable the following attributes: Remove xmlns, remove raster images, round/rewrite number lists, remove unknowns & defaults, replace duplicate elements with links, sort attrs, prefer viewbox to width/height, remove style elements, and remove script elements.

I also recommend using the filtered version of HABPanel: https://community.openhab.org/t/solved-habpanel-sluggish/81756/27

Requires Swiss911 Font, not included. Some devices don't support installation of fonts, so for those devices I changed the relevant text items to paths using Inkscape.

Icon attribution notice: some weather icons are included. Icons made by <a href="https://www.flaticon.com/authors/srip" title="srip">srip</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>

My work is based on the following SVG, released under CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/ 
https://en.wikipedia.org/wiki/LCARS#/media/File:Lcars_wallpaper.svg

Also, a big thanks to Alexander Richardson, whose great work on LCARS graphics has inspired me. https://lcarsgfx.wordpress.com

Finally, thanks to Michael Okuda for the original design of the LCARS graphics.