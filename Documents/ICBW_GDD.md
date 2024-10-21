# Game Design Document (GDD)

## Game Overview

**Title:** It Could Be Worst

**Genre:** Survival, Resource Management

**Platform:** PC

**Target Audience:** Players who enjoy survival games, both casual and hardcore (ages 12+)

**Theme:** Survival in a harsh environment characterized by alternating cycles of ***calm*** and ***storms***, with resource management and strategies to face severe weather conditions.

**High Concept:** The player must survive in an environment where calm (day) and storm (night) cycles challenge their ability to gather resources and survive. During the calm, they can explore, gather resources, and prepare for the storm. During the storm, they must stay near the fire to keep warm and find ways to survive the adverse conditions.

**Inspiration:** Dome Keeper, Don't Starve, DREDGE, Subnautica.

**Development Software:** Unreal Engine, Blender

## Gameplay Mechanics

Here is the list of main features translated into English:

### Main Features

#### 1. **Day/Night Cycle (Calm and Storm)**
   - **Description:** Implementation of the alternating cycle between calm and storm phases. During calm (day),
   - the player can explore, gather resources, and prepare. During the storm (night), the player must survive 
   - near the campfire.
   - **Specific Features:**
     - Timer for phase duration.
     - Visual transitions (e.g., changes in lighting and weather conditions).

#### 2. **Temperature Management**
   - **Description:** The player must maintain an optimal body temperature to avoid damage or death. The 
   - temperature drops during the storm and is restored by staying close to the fire.
   - **Specific Features:**
     - Player temperature indicator (HUD).
     - Temperature effects on gameplay (e.g., movement slowing down, health loss).

#### 3. **Resource Gathering System**
   - **Description:** During the calm phase, the player can gather resources such as wood, food, and materials
   - to craft items or repair structures.
   - **Specific Features:**
     - Different types of resources with unique properties (wood for the fire, food for health recovery).
     - Specific gathering areas (forest, cave, frozen lake).

#### 4. **Crafting System**
   - **Description:** The player can use gathered resources to create tools, upgrade structures, or repair the
   - campfire.
   - **Specific Features:**
     - Crafting menu with recipes for various items.
     - Craftable tools that affect activities (e.g., axe for chopping trees).

#### 5. **Campfire Management**
   - **Description:** The campfire is the focal point of survival during storms. The player must keep the fire
   - burning to maintain warmth.
   - **Specific Features:**
     - Consumption of wood to keep the fire going.
     - Visual and audio indicators of the fire's level.

#### 6. **Dynamic Threats**
   - **Description:** During storms, the player may face random events such as strong winds, snowfall, or animal
   - attacks.
   - **Specific Features:**
     - Management of dynamic events that require quick actions.
     - Impact of threats on the campfire or structures (e.g., extinguishing the fire, damaging the shelter).

#### 7. **Exploration and Diverse Biomes**
   - **Description:** The world is divided into unique biomes with different resources and dangers (forest, 
   - cave, frozen lake).
   - **Specific Features:**
     - Variety of resources and wildlife in each biome.
     - Unique exploration mechanics for each area (e.g., the ice on the lake can break).

#### 8. **HUD and User Interface**
   - **Description:** The user interface displays key information such as health, temperature, inventory, and
   - the game phase timer.
   - **Specific Features:**
     - Dynamic inventory display.
     - Indicators for the game cycle and temperature.

#### 9. **Progression and Upgrades**
   - **Description:** Possibility to improve the character's abilities, structures, or tools to face future 
   - storms.
   - **Specific Features:**
     - Progression system that rewards the player for surviving.
     - Gradual unlocking of new crafting recipes or upgrades.

These features cover the main mechanics and essential dynamics needed to create the survival experience 
envisioned for the game. We can expand or modify the list based on further details or ideas that may arise
during development.

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

--
 
## Technical Specifications

### **Minimum Requirements**
   - **Operating System:** Windows 7/8/10/11 (64-bit)
   - **Processor:** Intel Core i3-3220 / AMD FX-6300
   - **RAM:** 4 GB
   - **Graphics Card:** NVIDIA GeForce GTX 660 / AMD Radeon HD 7870 (2 GB VRAM)
   - **DirectX:** Version 11
   - **Storage:** 5 GB available space

### **Recommended Requirements**
   - **Operating System:** Windows 10/11 (64-bit)
   - **Processor:** Intel Core i5-8400 / AMD Ryzen 5 2600
   - **RAM:** 8 GB
   - **Graphics Card:** NVIDIA GeForce GTX 1060 / AMD Radeon RX 580 (4-6 GB VRAM)
   - **DirectX:** Version 11 or higher
   - **Storage:** 5 GB available space

### **Scalable Graphics Options**
   - **Graphics settings:** Allow players to adjust details such as texture quality, visual effects, resolution, and shadows. This will ensure a 
   - good experience on lower-end systems while reducing GPU and CPU load.
   - **Dynamic resolution:** Implement dynamic resolution scaling to maintain a target frame rate.
   - **Widescreen and ultrawide support:** Compatibility with different screen resolutions, up to 4K for more powerful systems.

### Recommended Resolutions
- **1280x720 (HD)** for basic configurations.
- **1920x1080 (Full HD)** as the main standard.
- **2560x1440 (QHD)** for mid-range setups.
- **3840x2160 (4K)** for high-end systems.
- **Ultrawide 21:9 and 32:9** for extended aspect ratio monitors.
- 
### Other Considerations
- **Level of detail management**. Not needed. The game use a top down fixed camera and all 3D models are lowpoly</font>
- **DirectX 11:** Still the standard for many configurations, ensuring compatibility with a wide range of graphics cards.
- **Testing on lower-end hardware:** Make sure the game is tested on machines with the minimum specs to ensure a smooth gaming experience.
- **Dynamic Resolution Scaling:** Implementing a dynamic resolution system can help maintain the target frame rate by automatically reducing the rendering resolution during complex scenes and restoring it when possible.
