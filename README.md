# Purpose
This Doc's purpose is to:
* Tell you what you need to know to find nades to practice. 
* Give you the minimum amount of info to use the Practice server.

This is meant to allow us to:
* Share nades easily
* Agree on which nades we want to know at minimum for each map
* A way to practice nade lineups at any time

For all the commands that can be used on the server: https://github.com/splewis/csgo-practice-mode#commands

For a video walkthrough of the commands: https://www.youtube.com/watch?v=ua_I30DTggQ 

# How To Start
On the server (connection info in Discord), once you connect you'll enable practice mode by typing the following in chat:
* ```.prac```
* ```.nades```
* ```.god```

*I also recommend setting a noclip bind in your Console, just type "bind q noclip" and use noclip to move around.* 

## Please Note:
* All the nades I added have a written description, you don't need to learn all the naming codes explained in the image below.
* Nades are saved to your profile, add whatever you nades want whenever you want and name them whatever you want, it won't mess up anything for anyone else.
* Example Jumpthrow and RunJumpthrow Binds are at the bottom at this page, if you don't have them already.
* If you think a nade should or shouldn't be "Default" (Nades we should all know), then just let me know.
* If you think you have a better lineup than one of the "Default" ones I added, let me know. Keep in mind:
  * How quickly you can throw the nade/How easy it is to lineup
  * How quickly the nade lands
  * Coverage - Are there gaps in smokes/mollies, and do Flashes cover everything they should?
  * What situations are they used in?
## Nade Names
Nades follow the same naming convention:
![image](https://user-images.githubusercontent.com/54295136/213258993-a74a7720-6306-44c3-b8c9-fee9b148a971.png)

## How to Search Nades by Category
You can look for specific names or parts of names using ".find" and you can lookup specific categories using ".nades [category name]" 

For the ".nades" command, you can ALSO filter by multiple categories:

To see any CT thrown nades on A site:
* ```.nades A Site&CT```

To see any T thrown Flashes that land in Mid:
* ```.nades Mid&T&Flash```

Please note: 
* You just use the ```.nades``` menu and go through the categories manually
* You can use "|" in the .nades [Filter] command as "OR"
  * *It has very limited use for when you want to see nades in either of two categories that do not overlap. If you think about it like a Venn diagram, "&" shows you everything where the circles overlap, and "|" only shows you what doesn't overlap in each circle.*

## How to Find Nades by Name

If you want to find nades without going through categories, you can do that by searching for the tags shown in the image above:
* Any Default Smokes on the Map that T's throw:
  * ```.find [*][T][S]```
* Any Run and Jump nades (not RunJumpthrow binds)
  * ```.find [R][J]```
* Any RunJumpthrow Bind nades:
  * ```.find [RJ]```
* All smokes on the map:
  * ```.find [S]```
  
# Binds

You put these in your autoexec.cfg file. For me the file location is: 

```C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg\autoexec.cfg```

Example Binds:
* Jumpthrow:
  * ```bind "z" "+jump;-attack;-jump"```
* RunJumpthrow:
  * ```
    bind "MOUSE4" "+forwardjumpthrow"
    alias "+forwardjumpthrow" "+forward;+jump;-attack"
    alias "-forwardjumpthrow" "-jump;-forward"
    ```
