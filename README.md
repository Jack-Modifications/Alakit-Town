DAYZ MOD - NAMALSK MAP ADDON

# MODS REQUIRED FOR THIS TO WORK:

1. [DayZ Editor Loader](https://steamcommunity.com/workshop/filedetails/?id=2276010135)
2. [Builderitems](https://steamcommunity.com/sharedfiles/filedetails/?id=1565871491&searchtext=Builderitems)


You may install this a couple of different ways:

# Installing via - .dze, .xml [DZE ONLY]
1. If you choose to install this via .dze (DayZ Editor Loader) please follow these instructions:

**DZE ONLY INSTALLATION COMING SOON, CURRENTLY MISSING AN IMPORTANT FILE!**

# Installing via - Init.c, .dze, .xml
2.  - IF you choose to install this via `init.c` you please follow these instructions.

Go to your server "mpmissions" folder and open "?????????.namalsk" folder which your server use.

After that, head over into `copy-to-mapgrouppos.xml` and copy the contents into your `mapgrouppos.xml` in your `mpmission` -> `????????.namalsk` main directory. **(I normally put it at the top in its own section.)**

After implementing the mapgrouppos.xml, Drag n Drop the `ALAKIT-TOWN-INIT.c` into your `????????.namalsk` main directory and put this at the top of your init.c: 
`#include "$CurrentDir:mpmissions/????????.namalsk/ALAKIT-TOWN-INIT.c"`

Once you have DayZ Editor Loader on your server then drag and drop `ALAKIT-DELETIONS.dze` to the `"EditorFiles"` folder. **(THIS IS CRUCIAL SINCE IT IS ONLY THE ORIGINAL NAMALSK DELETIONS IN THE .DZE FILE, NOT THE OBJECTS FROM `ALAKIT-TOWN-INIT.C`)**

and add this to the end in main function: `SpawnAlakitTown();`

It should look similar to the following:
![image](https://github.com/Jack-Modifications/refactored-octo-happiness/assets/102194777/cc68c2e8-88c4-4f36-885b-6ab5f0b625c2)
