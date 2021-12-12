# LMPGames_LayeredHPGauges
Version 0.5A

Demo Available: Yes [LMPGames_LayeredHPGauges_Demo_V0.5A.zip](http://lmpgames.com/RMMV/Plugins/LMPGames_LayeredHPGauges_V0.5A_Demo.zip)

Project Available: Yes [LMPGames_LayeredHPGauges_Project_V0.5A.zip](http://lmpgames.com/RMMV/Plugins/LMPGames_LayeredHPGauges_V0.5A_Project.zip)

Conflicts: None identified thus far

Terms of Use: Free non-commercially or commercially; just give credit

<p align="center"><img src="https://i.ibb.co/7nC5g1w/hpg-img1.png"/></p>

## What is this?
Every wanted to spruce up your battle screen?  Maybe you wanted to have something different for a boss battle?  Well look no further, this plugin can do that and a bit more!


## Installation Instructions
Drop the plugin file into your plugins folder, add it into your plugins list in your project in the editor, configure the plugin settings, set up enemy note tags.  You're Done!


## Current Features Overview
### Features in V1.3.5
- Unlimited Gauges
  - Create as many layers as you want, just make sure you have colors assigned for each layer.



- Color Gradient Layers
  - Each layer has a starting and ending color set up in the plugin settings.  This is completely customize able and supports any number of layers.



- Gauge Customization
  - You are able to change both the font size for the gauge and the gauge thickness.  Currently these are global settings and apply to every gauge.



- Battle Screen Object Offset
  - For certain battle scene elements that might get in the way of the gauges, there is a setting to add an offset to these.  Currently just the log window position is modified but more can be added upon request or instructions can be added for enterprising devs to add new items on their own.



- Gauge Visibility
  - Gauges can be set to show for every enemy, no matter the note tag settings, or they can be set to respect the note tags.  As such, its possible to configure boss battles with non-boss enemies and have the non-bosses have no gauge.



- Multiple Display Mode
  - Includes four information display modes; one that shows the enemy name and % of hp remaining, one that shows the name/current hp/% left, one that shows the name and current/max hp/% left, and a final one that shows only the name and no other health information.
    - Mode 1:  <p align="center"><img src="https://i.ibb.co/zstD2YQ/lhg-m1.png"/></p>
    - Mode 2:  <p align="center"><img src="https://i.ibb.co/wJ5Yvy9/lhg-m2.png"/></p>
    - Mode 3:  <p align="center"><img src="https://i.ibb.co/5FGdpFr/lhg-m3.png"/></p>
    - Mode 4:  <p align="center"><img src="https://i.ibb.co/HVG27wR/lhg-m4.png"/></p>





### Parameters
There are a total of eight plugin parameters to customize the plugin with.  I will list them and their functions.

- Number of Layers
  - This setting allows you to determine the max allowable number of layers to use for gauges.  The default setting is 5.  There is no maximum limit.
- Layer Gradient Start Colors
  - This setting sets the starting gradient colors that will be used for the left side of the gauge.  You must have the same number as the maximum layer setting.  It is formatted as a list of hex codes.
- Layer Gradient End Colors
  - This setting sets the ending gradient colors that will be used for the right side of the gauge.  You must have the same number as the maximum layer setting.  It is formatted as a list of hex codes.
- Gauge Font Size
  - This setting allows you to set the font size used for the guage.  The default setting is 18.
- Gauge Height
  - This setting allows you to modify the height of the gauge.  Please note that when more than one line of gauges is displayed, this setting can cause some overlapping.  A fix is in the works.  The default setting is 8.
- Display Item Offset
  - This setting allows you to set the offset for other battle screen elements near the top of the screen.  Currently it only impacts the window log, but more can be added per request or a tutorial on adding more can be created for custom UI elements.  The default setting is 10.
- Only ShowGauges on Note Tag
  - This setting forces gauges to respect note tags.  If no note tag is present, no gauge will be generated for that enemy.  The default for this setting is true.
- HP Display Mode
  - This setting allows you to switch between guage information display modes.  Please note that only mode 1 works when many gauges are on screen; the others do not fit or require lower font sizes to fit.



### Plugin Commands
None, yet.



## HP Gauge Note Tag
The note tag goes into the enemy note box and is formatted like this:

Example:
```
<LMPHPGauges>
Layers:5
ShowLayers
</LMPHPGauges>
```

Layers sets the number of layers that the enemy gauge will use.
ShowLayers allows you to set if the enemy will generate a gauge.  You can also leave the note box blank.  This note tag attribute is more for use when the plugin commands and scripting functions are added to allow you more control over when the guage can be displayed.



## Planned Features
- Make enemy gauges be deleted when they die
- Plugin commands and script functions for greater control
- Custom font support
- *conceptual* Image overlay support



## Conflicts
None found as of yet

## Version Changelog
- Version 0.5 Changelog:
  - Initial version of the plugin
