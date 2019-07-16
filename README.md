# Maperitive_rules_scripts
David South
 
To see what maps created with this process actually look like, go to the wiki for this repo.

### What is Maperitive?
[Maperitive](http://maperitive.net/) is a useful free tool for accessing OpenStreetMap data and creating maps. It functions differently than most other mapping programs, so here is a quick guide:
* [OpenStreetMap](www.openstreetmap.org) is a massive crowd-sourced worldwide dataset that evolves as users create and edit features. It uses .osm and similar files, based on [specific tags and features](https://wiki.openstreetmap.org/wiki/Map_Features) that the community defines, such as `place=city`, `highway=motorway`, or `natural=hot_spring`. These function very differently than traditional shapefiles, vectors, and rasters, and special methods are required to use these data.  
* OpenStreetMap data is free to use for personal and commercial projects, with very few restrictions. It is licensed under the [Open Data Commons Open Database License (ODbl)](https://opendatacommons.org/licenses/odbl/). Make sure you don't misuse the license.
* Read the [Two Minutes Introduction to Maperitive](http://maperitive.net/docs/TwoMinutesIntro.html) then the [Ten Minutes Introduction to Maperitive](http://maperitive.net/docs/TenMinutesIntro.html). The documentation for Maperitive isn't the best, many functions are undocumented or the documentation is incomplete, so beware. You can always search the [Google Group](http://groups.google.com/group/maperitive) for help.
* Maperitive displays OpenStreetMap data, but does not change the source data, only displaying it in different ways. You cannot create or edit features using Maperitive.
* Maperitive uses *rulesets* to determine how to display the data. These are `.mrules` files using the special coding language unique to Maperitive. [See rulesets documentation here](http://maperitive.net/docs/Rulesets.html).
* You may have changed rulesets on Maperitive and thought "Hey now, nothing is changing on the map! The heck!". Do not fret. This probably means that you are trying to change the symbology of the basemap, which won't work. Try downloading a chunk of OpenStreetMap data as an `.osm`, `.osm.pbf`, or similar file. Then load that up in Maperitive using `File > Open Map Sources`, then hide the basemap in the Map Sources tab in the bottom right. Now reload those rules.

### How do I use these scripts?

To use these `.mscript` files, first open them in a text editor like Notepad++. Look at them to see what they do. Don't go using scripts if you don't understand what it does, that way lies madness and error messages.


1. Open Maperitive.
2. Edit and customize the scripts so that the file paths are correct and it shows you the areas that you care about at the proper zoom levels.
3. Run the script with `File > Run Script`.
4. Check that the outputs are what you wanted.

### Where can I find the cool icons?

[Game-icons.net](https://game-icons.net/) has amazing icons licensed under Creative Commons. Check the license for each icon, but as far as I know they can all be used personally or commercially as long as you follow the details of the license. 

### How do I add in my own locations?

As stated in the Maperitive explanation above, Maperitive does not create locations. You can, however, display GPS data in Maperitive, in conjunction with OSM data. 

Unfortunately, the simplest way to do this is to start hiking around to all the places you want to map, using a personal GPS device to record the coordinates of each location, then compile all the relevant locations into a `.gpx` file. Better get out there, you got a long way to go. Nobody said making maps was easy.

Just kidding. You can use [this site](https://www.gpsvisualizer.com/draw/) to pick out locations from the comfort of your computer, and it will export a `.gpx` file, perfect for displaying in Maperitive. Now you just got to choose how Maperitive should display the data, by adapting the [ruleset for GPS data](http://maperitive.net/docs/Querying_GPS_Data.html).
