Easier Pantheon Practice

# Description:
A mod that makes practicing in HoG easier. It adds many features some of them include, allowing you to press a key to reload bosses much quicker, matching the health and damage of bosses with P5, and giving you the ability to do fury practice in HoG. There are more but you can read the readme for that :)

# How to use
- Download this mod, the Modding API and SFCore from the modinstaller.
- To change the settings, pause the game in Hall of Gods and click on the buttons to increment the setting / bind a key. There isn't a way to decrement the counter so if you want to go back, just click on it until it turns to 0 (which will happen after it crosses the max value)
- To practice a Pantheon 5 boss, fight ascended. To Practice a Pantheon 1-4 boss, fight attuned.  
- If a key isn't registered using the GUI, go to the saves folder and add an [acceptable input](https://gist.github.com/TheMulhima/63a241194bfb95828ed6f46d9b09d449) in the respective keys to add a key bind. e.g.  `Key_Reload_Boss = "z"`.

# Features Explanation
## Settings
### To use: Click on the button in the GUI to increment the setting.
- remove_health -> removed the specified value of health each time a boss scene in HoG is loaded. 
#### Fury can be setup on each boss load by setting remove_health to your max health - 1.
- lifeblood -> add the specified amount of lifeblood each time a boss scene in HoG is loaded.
- soul -> add the specified amount of soul each time a boss scene in HoG is loaded. The GUI will only allow adding 33 soul each time the button is pressed. <br />If you want less (because you are using soul twister) you can do that from the settings file.
- hitless_practice -> makes you die in 1 hit to bosses. <br />The advantage of using this over radiant fights is 1. bosses have same health as p5 and 2. it gives the ability to use the other features of the mod like adding soul or quickly reloading bosses.
#### Note: Each click on the button will increment the setting. So, to get from remove_health:0 to remove health:8, click on the button 8 times. To get to a lower value like from 8 to 1, press the button 2 times (8 -> 0, 0 -> 1 (8 is the max value for remove_healh if you have 9 health))
## KeyBinds
### To use: Click on the button in the GUI to change the bind.
- Key_Reload_Boss -> Press this key during a boss fight to quickly reload the boss. <br />Mostly done at the end just as the boss dies. <br />Note that after pressing the reload key, you won't be able to return normally after you kill the boss. You will need to press the "Key_return_to_hog" or use dreamgate. Just for reference, using this takes 2 seconds to load a boss when using this key. On the other hand, doing it normally takes around 15 seconds. <br />(Note: where the dream gate is placed doesn't matter as performing a dreamgate (holding up + dreamgate) in a boss scene will teleport you to HoG regardless).
- Key_return_to_hog -> Equivalent to dream gateing but much faster and doesn't burn your eyes by showing a white screen.
- Key_teleport_around_HoG -> Teleports you around HoG. It alternates between the bench and gpz statue.
#### To unbind: Click on the button on the GUI then press esc key to close the pause menu.
##Other Settings
#### These are only found in the settings file which can be found in the [saves folder](https://github.com/TheMulhima/Speedrun-Tricks-Visual-Helper#saves-folder)
- remove_ingame_menu -> if true, removes the GUI.<br />Maybe becuase it comes in the way idk. mostly keep it to false becuase GUI >>>> Settings file.
- Dont_change_boss_health -> If you only want settings to be added <br />For example: to practice a modded boss
- allow_reloads_in_loads -> Allows you to use reload boss key in loads. NOTE: May break stuff so use it at your own risk.

 # Common use cases:
- Practice fighting in pantheons with **Fury of the Fallen**.
- The hotkeys (especially the reload boss) can be used to lower waiting time in loading screens.
- It can be used to practice specific bosses in P5 such as **Collector**. (also compatible with toggleable bindings mod for AB practice)
- The hitless option allows practice for hitless pantheons.

#Known Issues
- Reloading boss before Pure vessels screams causes HUD to disappear (fix: reload).
- Using allow reload during loads causes knight to be invisible for some time
- Using allow reload during loads causes lifeblood to not apply
- in absrad, remove_health doesnt work
Note: IMO thats not a bug because you cant start Abs Rad without full health anyways (and this mod is meant to simulate pantheons in HoG). If you disagree, you can message me and ill try to fix it.

# Other:
- The mod only works in Hall of Gods and doesn't affect pantheons or other areas of the game.
- The mod affects bosses of health. Needless to say, it shouldn't be used with other modded boss.
- To unbind any key, press the button on the GUI and press esc to close the pause menu.
- If you find any bugs or have any suggestions, you can message me on discord at Mulhima#2695.

# Dependancies:
- This mod depends on Modding API (Obviously) and SFCore.
# Credits
- Thank you to 56, RedFrog and SFGrenade for some of their code and zuiivel and nadva for their help.
