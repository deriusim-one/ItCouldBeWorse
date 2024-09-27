# Game Design Document (GDD)

## Game Overview

**Title:** It Could Be Worst

**Genre:** Survival, Resource Management

**Platform:** PC

**Target Audience:** Players who enjoy survival games, both casual and hardcore (ages 12+)

**Theme:** Survival in a harsh environment characterized by alternating cycles of ***calm*** and ***storms***, 
with resource management and strategies to face severe weather conditions.

**High Concept:** The player must survive in an environment where calm (day) and storm (night) cycles challenge 
their ability to gather resources and survive. During the calm, they can explore, gather resources, and prepare 
for the storm. During the storm, they must stay near the fire to keep warm and find ways to survive the adverse 
conditions.

**Inspiration:** Dome Keeper, Don't Starve, DREDGE, Subnautica.

**Development Software:** Unreal Engine, Blender

## Gameplay Mechanics

### Core Gameplay Loop:

The game alternates between two states: **calm** (<font color="red">180 seconds</font>) and **storm** (<font color="red">120 seconds</font>).
1. During **calm**, the player can **explore** the environment, gather resources, and prepare.
2. During the **storm**, the player must stay near the fire to **survive** the freezing cold and manage resources like wood to keep the fire burning.

#### Exploration (Calm)
- Gather natural resources (wood, <font color="red">food</font>, tools, materials).
- Interact with the environment (build shelters, prepare the campfire).
- Prepare for the impending storm.
	
#### Survival (Storm)
- Stay near the campfire to maintain body temperature.
- Manage the consumption of wood to keep the fire going.
- Face threats (enemies, weather events, structural damage).
- <font color="red">Craft tools and necessary repairs.</font>

### Core Mechanics:

- **Temperature Management:** The player must stay near the fire to avoid freezing to death during the storm.
- **Resource Gathering:** The player explores the game world to collect essential resources during the calm.
- <font color="red">**Crafting and Repairs:** Ability to create tools, objects, and repair damaged elements (like the campfire or shelter).</font>
- **Dynamic Threats:** During the storm, random events like strong winds or animal attacks occur, requiring real-time player reactions.


## World Design

### Environment:

- The world is centered around the campfire (the player's survival hub).
- **Biomes** to explore during the calm phase:
	- **Forest:** Main source of wood and food.	
	- <font color="red">**Caves:** Safe refuge but with limited resources.</font>
	- <font color="red">**Frozen Lake:** Dangerous area with rare resources.</font>

### Dynamic Events:

- During the **storm**, events such as gusts of wind and heavy rain can influence gameplay (e.g., making the fire burn out faster).
- Possible encounters with **animals** or **creatures** that approach the fire or attack the player.

## Player Mechanics