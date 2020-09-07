# PlanetSearch3Plans

Outline
-------

1. Everything will be **pixalated** even text. (Yes I'll have to create a special pixelated font just for my game) 
2. Helix (the main character) will travel through space and explore planets
3. All the gameplay will be split into 8 chapters or worlds that each will take at least **1 hour** to play through (max 3 hours) 

Specific game design decisions
------------------------------

- There are now a few different types of collectibles:

    - Currencies
    - Grouped collectible
    - Key items 
    - Power ups
    - Abilities

 - Each of these will inherit from the collectibles class

- **Which means**: Power ups are now split into 2 categories; the temporary ones (Power ups) and the permenant ones (abilities)
(TODO: Elaborate more on this later)

- Jumping and falling:
    
    - You can now control **exactly** how high you jump. As soon as you release the jump button/key you will fall back down
    - If you fall to the bottom of a level (or fall in something really dangerous you **can't** walk in) you will be put 
    back on the last solid static piece of ground, block... whatever

- You'll now collect exp or score points after defeating **any** enemy.
    
    - When you collect enough exp or score points, you'll level up, which means you get to chose what to upgrade (or in 
    some cases just your hp/atk whatever will just take turns get increased) 
    something (like hp, atk whatever), then your lvl will increase by 1

    - Bosses force you to level up (or in some cases just give you like a heart or 5 hp or something related to health)

- Keys that unlock boss doors will have a different image so you can tell it's a boss key and be separate from normal keys.

- Things like ladders will stand out from the background so you can see them
- Doors and things like blocks will be styled differently to match their environment
- Two things that go together will be styled so it's obvious. For example, boss key to boss door
- Dying in this game won't be so easy or quick, if you do die you'll get a game over screen then your only option is to 
return to the title screen

- There will be shops
- You can buy items that do stuff like temporary attack up or rpg-like elements/action commands

- In space and on planets you will be able to get maps through different means to find your way around.
otherwise you won't (probably) be able to find your way around

- On planets there will be alien enemy camps that if you defeat you'll get something good and sometimes you'll get a different item
like a map for that planet

- You can buy stuff from a resident of a planet like a guy who sells stuff like maps

- Bosses:

    - In order to get to the boss of a planet you'll either have to wander around until you find the boss or you can buy maps to help you.
    - Once you defeat a boss you'll get:
        - Exactly enough exp to level up and heal you completely.
        - Star fragments. A sort of fuel (star fragments) for your spaceship.
        - Ammo for your guns.
        - A new ability. (if you didn't get one in that dungeon or for some other reason)
        - A map to the next planet to go to (remember you have to do the planets in order, if you find a planet by accident then your abilities will limit you to what you can do there)


- In space / other:

    - You have a limited amount of fuel (star fragments) and ammo and what's in your inventory.

    - You can shoot asteroids to get more fuel (star fragments) but they are rare and you have to grind to find them but they do give you ***plenty* of fuel**
    - To get more ammo try kill alien space ships.

    - Gems will be on planets or dwarf planets and you can collect them for well I haven't decided yet. I think has to do something with the ending of this game. 

- Guns:

    - Through out the game you can get different guns and trade guns. But they all have limited ammo.

- Your ship:

    - You'll have a new ship.
    - You can take your ship to a certain area for upgrades (that place/cutscene with the guy that "repairs"/upgrades your ship) 
    but it's **VERY** far away and you need a map to it. 
    - At first you'll have to ride on solar winds (since you'll have a solar sail, also if you go to a star you can recharge your 
    ships batteries using solar panels (which is crucial for your ship to function)) they are very slow at first but speed up overtime. And some times 
    won't work if you're too far away from a star.

    - Your ships has stats:
        - Hp
        - Fuel (star fragments) (ways to use your fuel: 
            1. Combustion (liquid, solid, hybrid) (oxygen, todo)
            2. Nuclear (fission, fusion) (uranium, plutonium)
            3. ion engine (todo) (electricity, xenon)
             )
        - Battery
    
    - If you see a gravity well you can use your quantum tractor beam (that you get much later in the game) to pull out goodies.

Implementation details
----------------------

- Phaser 3/4 will be used
- Matterjs for physics
- Some plugin for ui... maybe?
- A fast version of the cartesian system will be used 
- A plug-in for a bridge between the cartesian system and Phaser 3/4 for space.
- The multiple layers of the cartesian system will be used for moving star effects
Tilemaps will be used, no more glitchy cartesian systems (unless it's in space or water to something)
- Careful game object heirarchies will be used
- Saving will be handled myself and save files will be as small and efficient as possible
- If a game object does not have an `oncollide` method I will not let it collide with anything
or collision **should** be defined
- Millisecond timers should be turned into a timer class so that when the game lags the same object won't get repeaditly created because of a constant time being mismatched with game fps 
- A flexible test environment will be created (meaning I can test parts of the game without having to play the entire game up untill that point)

What software will be used to create the game- You have a limited amount of fuel (star fragments) and ammo and what's in your inventory.

- You can shoot asteroids to get more fuel (star fragments)

- Gems will 

----------------------------------------
- Visual Studio code with Phaser 3/4 intellisense
- Piskel (sprites)
- Tiled (levels)
- Bfxr (sound fx)
- FL studio/Famitracker/milky tracker for music

Storyline
---------
Keep a compelling storyline to keep the player playing!
Helix will get a new ship well his ship that's been so repaired because it was broken so badly it looks completely different and brand new.
There's even a place Helix goes to get this to happen. Well it's sort of a cutscene.
Also your ship's map database has been erased somehow. 