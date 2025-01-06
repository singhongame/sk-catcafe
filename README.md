# sk-catcafe

This resource was created as a QBCore only for UWU/CatCafe Restaurant Script and the jobs can be configured in config.lua easily.

Features/Configuration:
- Job Name Configurable
- Total of 4 Tray Configurable
- Slots, Weigts of All Trays
- Slots and Weights of Fridge
- Toggle Duty Location
- Order Items
- Add As many Custom Items As Possible 


## Installation

- Download the script
- For QBCore Add item Name Into Items.Lua
```
    -- cat cafe items
    bmochi 						= {name = 'bmochi',  	     			label = 'Blue Mochi',	 			weight = 100, 		type = 'item', 		image = 'mochiblue.png', 		unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['hunger'] = math.random(40, 50) },
	pmochi 						= {name = 'pmochi',  	     			label = 'Pink Mochi',	 			weight = 100, 		type = 'item', 		image = 'mochipink.png', 		unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['hunger'] = math.random(40, 50) },
	gmochi 						= {name = 'gmochi',  	     			label = 'Green Mochi',	 			weight = 100, 		type = 'item', 		image = 'mochigreen.png', 		unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['hunger'] = math.random(40, 50) },
	omochi 						= {name = 'omochi',  	     			label = 'Orange Mochi',	 			weight = 100, 		type = 'item', 		image = 'mochiorange.png',		unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['hunger'] = math.random(40, 50) },

	--Drinks
	bobatea 					= {name = 'bobatea',  	     			label = 'Boba Tea',	 				weight = 100, 		type = 'item', 		image = 'bubbletea.png', 		unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['thirst'] = math.random(40, 50) },
	bbobatea 					= {name = 'bbobatea',  	     			label = 'Blue Boba Tea',	 		weight = 100, 		type = 'item', 		image = 'bubbleteablue.png',	unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['thirst'] = math.random(40, 50) },
	gbobatea 					= {name = 'gbobatea',  	     			label = 'Green Boba Tea',	 		weight = 100, 		type = 'item', 		image = 'bubbleteagreen.png', 	unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['thirst'] = math.random(40, 50) },
	pbobatea 					= {name = 'pbobatea',  	     			label = 'Pink Boba Tea',	 		weight = 100, 		type = 'item', 		image = 'bubbleteapink.png', 	unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['thirst'] = math.random(40, 50) },
	obobatea 					= {name = 'obobatea',  	     			label = 'Orange Boba Tea',	 		weight = 100, 		type = 'item', 		image = 'bubbleteaorange.png', 	unique = false, 	useable = true, 	shouldClose = true,   	combinable = nil,   description = '', ['thirst'] = math.random(40, 50) },
	
```

- Add the below to qb-core/shared/jobs.lua
```
	catcafe = {
		label = 'CatCafe',
		defaultDuty = true,
		offDutyPay = false,
		grades = {
            ['0'] = { name = 'UWU Recruit', payment = 500 },
			['1'] = { name = 'UWU Junior Chef', payment = 700 },
			['2'] = { name = 'UWU Bartender', payment = 900 },
			['3'] = { name = 'UWU Exp Chef', payment = 1100 },
			['4'] = { name = 'UWU Manager', payment = 1500 },
			['5'] = { name = 'UWU Senior Manager', isboss = true, payment = 1900 },
			['6'] = { name = 'UWU CEO', isboss = true, payment = 2200 },
        },
	},

```

- Verify that the job name and the Config.jobname both should be same. 

- Copy and paste the images from /image directory to qb-inventory\html\images
- Put script in your `resources` directory.
- Make sure to add the script in server.cfg: 
```
ensure sk-catcafe
```
- Make sure the script are running in your txAdmin Panel

- To make items Consumable make sure to add the items name in jim-consumables or qb-smallresources. If you need help then reach out to our discord support. 


## Dependency
1. qb-core
2. qb-Inventory

### Extra Information
- Inventory image included in the `image` directory

### Upcoming
- Payment integration and Support
- Crafting
- Consumption In-Built Support
- Ox Inventory Support

## Preview


# Support

# Buy Here: https://kumarsk.tebex.io/package/6149569

