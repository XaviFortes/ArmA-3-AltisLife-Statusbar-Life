# ArmA-3-AltisLife-Statusbar-Life
##### Statusbar for your AltisLife TanoaLife any life server that you want to implement a statusbar easily


## Tutorial

1. Paste the files following the **structure**
```sqf
Mission.folder
+---core 
|   \---karasu
|       \---karasu_statusbar.sqf
|       
+---dialog
|   \---karasu_statusBar.hpp
|      
|          
+---textures
   \---icons
       \---karasu_statusbar
           \---civ.paa
            |--compass.paa
            |--cop.paa
            |--fps.paa
            |--health.paa
            |--hunger.paa
            |--med.paa
            |--stamina.paa
            |--thirst.paa
            |--uptime.paa
```
2. Go to your mission's root directory and open **init.sqf** and add the following:
> [] execVM "core\karasu\fn_statusBar.sqf";

It should look like this:
```sqf
[] execVM "briefing.sqf"; //Load Briefing
[] execVM "KRON_Strings.sqf";
[] execVM "core\karasu\fn_statusBar.sqf";
```

Navigate back to your mission's root directory and open up **description.ext** and add the following underneath class **RscTitles**
> #include "dialog\karasu_statusBar.hpp"

And now it should look like this:
```sqf
class RscTitles {
	#include "dialog\progress.hpp"
	#include "dialog\hud_nameTags.hpp"
	#include "dialog\hud_stats.hpp"
	#include "dialog\karasu_statusBar.hpp"
};
```

##### Now the installation it's complete :D
