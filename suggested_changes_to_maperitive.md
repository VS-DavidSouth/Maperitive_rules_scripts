# Suggested changes to Maperitive
Written by David South

Maperitive is a wonderful, useful mapping tool for OpenStreetMap data. It is a labor of love by a single person, and they do a great job. 

But, as it says in the Maperitive ReadMe,
*"While it will probably not burn your computer or kill your pets, Maperitive is highly undocumented* 
*and almost certainly full of bugs. Also, it's not very user-friendly.*
*Keep in mind that a lot of things will probably change (and hopefully improve) in the near future."*

So here are my suggestions for how Maperitive can be further improved.

## Major Issues
* As far as I can tell, `text-offset-vertical` is completely non-functional, as is `text-offset-horizontal`. According to *the internet* it worked fine for Maperitive v2.4.1, but no longer works for v2.4.3.

## Minor Issues
* I am not sure if this exists already, but it would be nice to have a way to sometimes show something over text. For example, large icons that are more important than street names.
* Label collision is really frustrating when you have a perfect map but you can't read some labels because they overlap. Implementing a fix for this would be very helpful.
* Similar to detecting label overlap, many times I try to export a map and there is a label that is partially cut off by the bounds of the exported image. This makes things look unprofessional and are not aesthetically pleasing. Ideally, there  could be a setting that could be used to tell Maperitive to not draw text/labels which were partially across printing or geometry bounds.
* It seems like there should be a better way to fix the [disappearing oceans issue](http://maperitive.net/docs/Rendering_Coastlines_And_Sea.html).

## Documentation Issues
* A guide to the general syntax of Maperitive would be great. Things like - instead of _, spaces in names are sometimes okay, but also function inputs are separated by spaces not commas, indentation level matters in rulesets, etc. As someone who cut my teeth in Python and R, it was a grind trying to get used to the syntax.
* More examples and explanation of the use of conditional logic, like `AND`, `OR`, `FOR`, `ELSEFOR`, `@if`, etc and what situations each can be used.
* I still am not clear on the actual functional differences between Geometry Bounds and Printing Bounds, and which should be used in which situations. I usually just set them to be the same.
* The page for [Querying GPS Data](http://maperitive.net/docs/Querying_GPS_Data.html) is very useful. It would be nice if it were explained that to specify tags with GPS stuff, you put it within the brackets when you define a feature, like `gpswaypoint[symbol=Airport]`. That took me quite a while to figure out.
* It is very unclear exactly what types of non-OSM data can be used in Maperitive. I found that GPS `.gpx` file can, but it would be really helpful to have an extensive list with a documentation page devoted to each.
 type of data that Maperitive can use.
 
## Added Functionality
* It would be nice to be able to have an `icon-opacity` parameter to make them partially transparent. 
* A warning could pop up when a user tries to change a ruleset but only has the default base web map in the Map Sources tab. Doubtless virtually all newbie users have made this mistake and were frustrated when it didn't change anything. You learn quickly that the rulesets only apply to downloaded data displayed in Map Sources, but that isn't immediately apparent and I had to do 20 minutes of searching to find why. This could easily drive off potential users who get frustrated and give up on learning to use Maperitive.
