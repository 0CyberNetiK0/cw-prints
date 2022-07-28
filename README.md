# cw-prints 🖨
This script enables player created business cards. Comes with a warp to an interior butthis can easily be ignored if you want to use it in any other fashion. Easilyconfigured in the *Config.Lua*.
In the future we plan to make it support any type of printable item (flyers etc)
# Preview 📽
[Video](https://youtu.be/CSYWQ2pf2a4)
# Config 🔧
**JobIsRequired**: Set to *true* if you want to lock this behind a job. Default is*false*\
**AllowedJob**: The job you want to be able to use it. Only needed if JobIsRequired is*true*\
**Locations**: Vectors for the warps and the interaction point\
**Texts**: Strings for the interaction point\
**Item**: The item that is created and added to your inventory\
**Cost**: Cost per card\

## Changing interaction shake
If you don't want to use the current warp and interior then all you need to do is add this event to wherever you want to call it: `"cw-prints:client:openInteraction"` This will open the interaction menu for the script. 
# Add to qb-core ❗
Items to add to qb-core>shared>items.lua if you want to used the included item
```
["business_card"] 					 = {["name"] ="business_card", 			  	  		["label"] = "A business card", 			["weight"] = 0, 		["type"] = "item", 		["image"] = "bctest.png", 			["unique"] = false,	 	["useable"] = true,			["created"] = nil,		["decay"] =nil, 	["shouldClose"] = false, ["combinable"] = nil,   ["description"] = "A businesscard"},
["coupon"] 					 = {["name"] = "coupon", 			  	  		["label"] ="Coupon", 				["weight"] = 0, 		["type"] = "item", 		["image"] ="coupon.png", 				["unique"] = false,	 	["useable"] = true,		["created"] = nil,		["decay"] = nil, 	["shouldClose"] = false, ["combinable"] =nil,   ["description"] = "A Coupon"},
["flyer"] 					 = {["name"] = "flyer", 			  	  		["label"] ="Flyer", 				["weight"] = 0, 		["type"] = "item", 		["image"] ="flyer.png", 				["unique"] = false,	 	["useable"] = true,		["created"] = nil,		["decay"] = nil, 	["shouldClose"] = false, ["combinable"] =nil,   ["description"] = "A Flyer"},

```
Also make sure the images are in qb-inventory>html>images
# Dependencies
* PS-UI - https://github.com/Project-Sloth/ps-ui/blob/main/README.md
* qb-target - https://github.com/BerkieBb/qb-target
## Developed by Coffeelot#1586 and Wuggie#1683
[More scripts by us](https://github.com/stars/Coffeelot/lists/cw-scripts)\
[Updates and Support](https://discord.gg/FJY4mtjaKr)
