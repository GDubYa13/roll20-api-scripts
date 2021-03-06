# Hexploration

_v1.1 Updates:_
* The script now has a chat menu interface.
* Implemented script configurations for hex colors.
* Implemented reveal distance configuration. When a token moves, it will also reveal hexes out to this distance.
* Hexes can now be named. When the named hex is revealed, it will announce that it has been discovered in the chat.
* Implemented inverted fill. This works like the ordinary polygon fill, except that every hex NOT in the selected polygons is filled instead.

This script allows GMs to draw a polygon on a hex-gridded map and fill in
each hex inside that polygon with an opaque hexagon. It's great for hex-based
maps where the PCs must explore and discover each area hex by hex.

## General Usage

This script's actions and configurations are accessible through its menu
displayed in the chat (Visible only to the GM).
To open the script's menu, activate the 'Hexploration_menu' macro installed
by the script.

Note that this script only works for maps whose grid types are set to either
'Hex (V)' or 'Hex (H)'. The opaque hexes will be aligned to the page's hex
grid.

When you move a token representing a character into an area concealed by a hex,
the hex will be revealed. If the script's reveal distance is set greater than 0,
then adjacent hexes out to that distance (in hex units) will also be revealed.

Watch https://raw.githubusercontent.com/Roll20/roll20-api-scripts/master/Hexploration/Hexploration.gif
for a short demo of the basics of how the script works.

### Rendering Hexes

To create a hex-filled area, first draw one or more polygons containing the
area you want filled with hexes. Then select the polygons and press the
'Fill Polygon' action from the script's menu. That's it!

### Naming Hexes

Hexes can be named to represent locations that are concealing. The names of
the hexes will be shown on the GM layer, invisible to the PCs. When a named
hex is revealed, it will announce that its location has been discovered in the
chat.

There are two ways to name locations hidden by hexes:

Before rendering the hexes using the 'Fill Polygon' action, create named tokens
with the 'white-tower' status representing the locations you want to conceal
with the hexes.

To name a hex that's already been rendered, select the hex and set its name
using the 'Name Hex' action from the menu.

## Actions

The script contains the following actions available from the script's chat menu:

### Fill Polygon

This renders hexes within one more more polygon areas.
Select one or more polygons, then use this action to fill their areas with
hexes.

### Inverse Fill

This works like the 'Fill Polygon' action, except that it renders hexes
everywhere on the page except inside the selected polygons' areas instead.

### Name Hex

This allows you to name a hex after it has been rendered. Select the hex you
want to name, then use this action to specify a name for it.

## Configurations

The script contains the following configurations that can be set from the
script's chat menu:

### Hex Color

This allows you to specify the color, border color, and label color of hexes.
This must be set before the hexes are rendered.

### Border Width

This sets the width of the border outlines on hexes. This must be set before
rendering the hexes.

### Reveal Distance

This specifies how far out (in units) hexes are revealed when a character
token is moved.

## Help

If you experience any issues while using this script or the trap themes,
need help using it, or if you have a neat suggestion for a new feature, please reply to this thread:
https://app.roll20.net/forum/post/6179141/script-hexploration
or shoot me a PM:
https://app.roll20.net/users/46544/stephen-l

## Show Support

If you would like to show your appreciation and support for the work I do in writing,
updating, and maintaining my API scripts, consider buying one of my art packs from the Roll20 marketplace (https://marketplace.roll20.net/browse/search/?keywords=&sortby=newest&type=all&genre=all&author=Stephen%20Lindberg)
or, simply leave a thank you note in the script's thread on the Roll20 forums.
Either is greatly appreciated! Happy gaming!
