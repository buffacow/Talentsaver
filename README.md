# Talentsaver v1.42 (for Vanilla WoW 1.12.1)
With Talentsaver you can save your current talent spec, and load the saved talent spec with an simple command.

It was initially created for my ViroUI pack but due to popular demand I released it independently.

# Showcase

Listing my custom saved talent templates
<img src="https://i.imgur.com/xf2IxW5.png"></img>

Loading an custom saved talent template
<img src="https://i.imgur.com/2aHFLDa.png"></img>

[![Talentsaver 1.4 Preview on Youtube](http://i.imgur.com/aNjG5bV.png)](https://www.youtube.com/watch?v=8au61bMst10 "Talentsaver 1.4 Preview on Youtube")

# Discussion
<a href="https://forum.nostalrius.org/viewtopic.php?f=63&t=15429"><b>Nostalrius Forum Thread</b></a>

# Chat Commands
- /talentsaver /talents or /ts
- /talents save name - to save the current spec as 'name'
- /talents load name - to load the template named 'name'
- /talents delete name - to delete the template named 'name'
- /talents list - to display a list of your saved Talent templates
- /talents delay number - to change the delay. 'number' in ms (eg. 'delay 400' for 400ms delay)
    Default Value is -1 which means the AddOn calculates the delay latency dependent (latency in ms/50*0.4)
- /talents stop - will stop if a template is being loaded right now

# Changelog
1.42 (28. November 2020)
- included the missing dependency libraries, Talentsaver now works as a standalone addon

1.41 (3. July 2015)
 - fixed the DoubleCheck process (delayed it)
 - the estimated loading value will now be increased by 2s to make it more accurate

1.4 (2. July 2015)
 - added a FuBarPlugin for easier usage
 - added a DoubleCheck (if the loading process is finished it will check if it's really finished, Lag Spikes could fail the process)
 - overhauled load, save and delete functions as well as few other functions and variables

1.3 (27. July 2014)
- added the 'stop' command
- completely remade the BUILD Variables and therefor saving&loading procedures
- fixed the loading procedure if points are already spent

1.2 (26. July 2014)
- changed the Spec Info Variables from string to table with 4 int values(!)
- deleting a spec will now completeley remove it from the LIST table and therefor the /list command
- on loading it will display an estimated loading time
- on loading it will now check how many points you have free and how much you need
--> it can now continue loading the template if you've already spent a few of the needed points correctly
(if you've spent them on your own or the loading process got stopped due to dc)

1.1 (22. July 2014)
- fixed the delay variable (from s to ms)
