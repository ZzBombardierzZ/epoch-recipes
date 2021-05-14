# Epoch-Recipes
Preview buildable items and recipes 


![GitHub Logo](http://puu.sh/HFZaU/85cde340c9.png)



### Prerequisites

```
Install the Trader Catalogue first!
a custom compliles.sqf, keyboard.sqf or another way to open the menu
```


### Install

In your **description.ext** at the bottom paste
(below chx_defines.hpp from the trader catalogue)

```
#include "scripts\recipes\chx_buildings.hpp" 
```

Save and close.





//-------------------------------------------------------------------------

In your **compiles.sqf** find

```
if (!isDedicated) then {
```

Somewhere below that paste

```
call compile preprocessFileLineNumbers "scripts\recipes\init.sqf";

```

Save and close.




//-------------------------------------------------------------------------

Next, open your **keyboard.sqf**, scroll to the bottom and above the last 
```
_handled
```

Paste

```
	if (_dikCode == 0x25) then { [] call building_catalog;	};	// Recipes (K) Button
```

Save and close.
//-------------------------------------------------------------------------






**Install Complete**




## Acknowledgments

Epoch devs
And everyone in the forums/discord for testing and helping.

