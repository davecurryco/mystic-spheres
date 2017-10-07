# Nautical Rules

## Ship Types

| Ship Type     |    Size    | Sea  | Crew | Pass | Cargo | Weapon |  AC  |  HP  |  DT  |   Ram |  Speed  |  Move   | Masts |  Sail  | Maneuver     |
| ------------- | ---------- | ---: | ---: | ---: | ----: | -----: | ---: | ---: | ---: | ----: | ------: | ------: | ----: | ------ | ------------ |
| Small Galley  | Gargantuan |   12 |   40 |      |    75 |  4/1/0 |   14 |  300 |  15  |   6d8 |   1/2   |  10/20  |    1s | Main   | Poor/Average | 
| Galley        | Colossal   |   12 |   80 |      |   150 |  6/2/0 |   15 |  400 |  20  |  8d10 |   1/3   |  10/30  |    1s | Main   | Clumsy/Poor  |
| Large Galley  | Colossal   |   12 |  120 |   20 |   200 |  8/2/0 |   15 |  500 |  20  | 12d10 | 1.5/4   |  15/40  |    2s | Main   | Poor/Average |
| Ironclad      | Colossal   |   10 |   80 |   10 |   100 | 12/4/0 |   17 |  600 |  25  | 12d12 | 1.5/2   |  15/20  |     2 | Main   | Clumsy/Poor  |
| Keelboat      | Gargantuan |   10 |    1 |    6 |   0.5 |  4/1/- |   15 |  100 |  10  |   3d6 |   1/1   |  10/10  |     1 | Main   | Poor/Average | 
| Launch        | Large      |    8 |    3 |    9 |   0.5 |  -/-/- |   12 |   60 |   -  |   2d4 |   1/1   |  10/10  |    1s | Main   | Poor/Average |
| Longship      | Colossal   |   16 |   40 |  150 |    10 |  6/1/0 |   15 |  300 |  15  |   5d8 | 1.5/3   |  15/30  |    1s | Main   | Average/Good |
| Outrigger     | Huge       |    6 |    1 |      |     2 |  -/-/- |   12 |   60 |   -  |   2d4 | 2.5/1   |  25/10  |     1 | Main   | Good/Good    | 
| Rowboat       | Large      |    4 |    1 |    3 |       |  -/-/- |   11 |   50 |   -  |   2d4 |   -/1   |   -/10  |     - | -      | -/Average    |
| Full Rig Ship | Colossal   |   18 |   40 |   20 |   150 | 10/2/- |   13 |  300 |  15  |   5d8 |   4/-   |  40/-   |     3 | Full   | Average/-    |
| Small Ship    | Gargantuan |   12 |   10 |   10 |    50 |  8/2/1 |   13 |  150 |  15  |   4d6 |   2/1   |  20/10  |     1 | Plain  | Poor/Poor    |
| Sailing Ship  | Colossal   |   16 |   30 |   20 |   100 | 10/2/1 |   13 |  300 |  15  |   5d8 |   3/-   |  30/-   |     2 | Plain  | Average/-    |
| Small Warship | Colossal   |   16 |   40 |   30 |   150 | 12/2/1 |   15 |  350 |  20  |   5d8 |   2/-   |  20/-   |     2 | Plain  | Average/-    |
| Warship       | Colossal   |   16 |   60 |   60 |   200 | 16/2/1 |   15 |  500 |  20  |   6d8 | 2.5/-   |  25/-   |     2 | Plain  | Poor/-       |

**Notes:**

* Sea = Seaworthiness
* Crew = Number required to move under oar for 1 watch/day or sail for 3 watches/day w/o exhaustion
* Cargo = Cargo capacity in tons
* Weapon = Weapon spaces Port,Starboard/Fore,Aft/Amidships
* DT = Damage Threshold
* Ram = Damage per 10 ft. relative speed; Ships w/o ramming prow take 1/2 damage from ram.
* Speed = Sail/Oar base speed in knots
* Move = Sail/Oar base movement in feet
* Masts = (s) indicates mast is shippable
* Sail = Maximum deployed sail
* Maneuver = Sail/Oar maneuverability class

## Movement

### Under Sail

#### Wind / Ship Speed Modifier (Knots)

| Force        | Wind Speed | Ship Speed | Ship Move  |  To Hit | Damage |
| ------------ | ---------: | ---------: | ---------: |  -----: | -----: |
| Calm         |          0 |          0 |          0 |         |        |
| Light        |       1d12 |         +0 |         +0 |         |        |
| Moderate     |    1d12+12 |       +1d4 |  +1d4 x 10 |         |        |
| Strong \*    |    1d12+24 |       +3d4 |  +3d4 x 10 |         |    2d4 |
| Gale \*      |    2d12+33 |       +3d6 |  +3d6 x 10 |      +2 |    4d6 |
| Tropical \*  |    2d12+60 |       +3d8 |  +3d8 x 10 |      +5 |    8d8 |
| Hurricane \* |        86+ |       +4d8 |  +4d8 x 10 |     +10 |  16d10 |

\* Each watch a sailing ship is operated in such winds, roll an attack against the Deployed Sail AC. Damage is to the ship's rigging.  

#### Deployed Sail

| Sails             |  Speed   |  Rig AC  | Description                                            |
| ----------------- | -------: | -------: | ------------------------------------------------------ |
| No Sail           |    -100% |       25 | Ship drifting with current unless anchored.            |
| Short Sail        |     -50% |       22 | Jibs and driver sail only. Basic move and maneuver.    | 
| Fighting Sail     |     -20% |       20 | Jibs, driver, and reefed topsails. Reefed is 1/2 sail. |
| Main Sail         |     -15% |       18 | Mainsail only.                                         | 
| Reefed Plain Sail |     -10% |       18 | Jibs, driver, reefed mainsails, and reefed topsails.   |
| Plain Sail        |       0% |       16 | Jibs, driver, mainsails, and topsails.                 |
| Reefed Full Sail  |     +10% |       14 | All above plus reefed topgallants and royals.          |
| Full Sail \*      |     +20% |       12 | All above plus full topgallants and royals.            |
| All Sails \*\*    |     +50% |       10 | Every scrap of duck on the wind!                       |

\* -2 to all maneuvering rolls due to speed  
\*\* -5 to all maneuvering rolls due to speed  

#### Wind Direction Speed Modifier

| Square Bearing | Hex Bearing | Square  | Fore/Aft |
| -------------: | ----------: | ------: | -------: |
|              1 |           1 |   -100% |    -100% |
|                |        2,12 |    -75% |     -60% |
|            2,8 |        3,11 |    -50% |     -40% |
|            3,7 |        4,10 |    -25% |     -10% |
|            4,6 |     5-6,8-9 |      0% |       0% |
|              5 |           7 |    -10% |      -5% |

#### Time to Change Sail (One Level)

| Crew Quality | Rounds  |
| ------------ | ------: |
| Lubbers      |       8 |
| Rabble       |       6 |
| Able Sailors |       4 |
| Sea Dogs     |       2 |
| Old Salts    |       1 |

Note: Times are halved on a ship with only 1 mast.

### Under Oar

The Oar Speed column on the Ship Type table gives the ship's speed in knots when under oar. 

### Movement Modifiers

#### Crew Speed Modifer

| Crew Quality | Modifier |
| ------------ | -------: |
| Lubbers      |     -25% |
| Rabble       |     -15% |
| Able Sailors |       0  |
| Sea Dogs     |      +5% |
| Old Salts    |     +10% |

#### Ship Condition Modifer

| Condition | Percent HP | Modifier |
| --------- | ---------: | -------: |
| Excellent |       100% |       0% |
| Good      |        80% |      -5% |
| Fair      |        60% |     -10% |
| Poor      |        40% |     -20% |
| Excerable |        20% |     -40% |

## Maneuver

### Manuverability

| Manuver            |     Good    |   Average   |    Poor    |    Clumsy    |
| ------------------ | ----------: | ----------: | ---------: | -----------: |
| Min. forward speed |       5 ft. |      5 ft.  |      5 ft. |        5 ft. |
| Move backward \*   |         Yes |        Yes  |        Yes |          Yes |
| Reverse \*         |      -5 ft. |    -10 ft.  |     -10 ft.|      -10 ft. |
| Turn               |   90°/5 ft. |   45°/5 ft. |   45°/5 ft. |   45°/10 ft. |
| Turn in place      | +90°/-5 ft. | +45°/-5 ft. | +45°/-5 ft. | +45°/-10 ft. |
| Max. turn          |         Any |         90° |         45° |          45° |

* When powered by oars only.


### Short Crew Modifiers

| % Crew   |  Actions   |      Time      |
| -------: | ---------: | -------------: |
|    < 30% | No Actions |     No Actions |
| 31 - 39% |         -3 |   3x (Tripled) |
| 40 - 49% |         -2 |   2x (Doubled) |
| 50 - 79% |         -1 | 1.5x (Slowed)  |
|    > 80% |          - |    No Modifier |

## Travel

Roll Weather for each 8-hour Watch, calculate Speed in knots, then lookup Distance traveled.

### Travel Per Watch

| Speed (Knots) | Distance (Miles) |
| ------------: | ---------------: |
|             1 |                8 |
|             2 |               16 |
|             3 |               24 |
|             4 |               32 |
|             5 |               40 |
|             6 |               48 |
|             7 |               56 |
|             8 |               64 |
|             9 |               72 |
|            10 |               80 |
|            11 |               88 |
|            12 |               96 |
|            13 |              104 |
|            14 |              112 |
|            15 |              120 |

## Combat

### Targeting

Direct-fire and targeted attacks can target either the ship's hull or its rigging. Attacks against hull are made against the ship's overall AC. The rigging has a separate AC, which depends on deployed sail.

Indirect-fire and area of effect attacks are made against the ship's overall AC.

### Relative Speed

#### Calculate Relative Speed

| Ships Moving                            | Relative Speed                          |
| --------------------------------------- | --------------------------------------- |
| Directly toward or away from each other | Add speeds                              |
| At 90° angle to each other               | Add speeds and divide by 2              |
| In same direction                       | Subtract speeds and take absolute value |

#### Relative Speed Attack Modifier

| Relative Speed | Modifier |
| -------------: | -------- |
|       < 40 ft. |        0 |   
|      40-60 ft. |       -2 |
|       > 60 ft. |       -4 |

### Damage

A sail ship's rigging comprises 25% of its overall hit point total. Attacks targeted at the rigging reduce its hit points directly.

#### Damage Effects

| Damage                      | Speed Reduced | Maneuver Reduced |
| --------------------------- | ------------: | ---------------: |
| 25% overall or 50% rigging  |       50%/25% |              1/- |      
| 50% overall or 100% rigging |      100%/50% |              4/1 |
| Crew 25% casualty           |       10%/25% |              1/1 |
| Crew 50% casualty           |       20%/50% |              1/2 |
| Crew 75% casualty           |       30%/75% |              2/3 |
| Crew 100% casualty \*       |      50%/100% |              3/4 |

\* A sail ship can move under a favoring wind with only a helmsman, but cannot tack or change sail.

* Speed Reduced = Reduction under Sail/Oar
* Manuver Reduced = Reduction in level under Sail/Oar

### Weapons

| Name               | Damage        | Range   | Properties          | Rate Fire | Fire Arc | Spaces | Crew |
| ------------------ | ------------- | ------: | ------------------- | --------: | -------: | -----: | ---: |  
| Light Catapult \*  | 12 (3d8)      | 100/500 | Ammunition, loading |   1/3 rnd |  45° fwd  |      1 |    1 |
| Medium Catapult \* | 16 (4d8)      | 150/600 | Ammunition, loading |   1/4 rnd |  30° fwd  |      1 |    2 |
| Heavy Catapult \*  | 20 (5d8)      | 200/800 | Ammunition, loading |   1/5 rnd |  15° fwd  |      2 |    4 |
| Ballista           | 12 (3d8)      | 120/480 | Ammunition, loading |   1/3 rnd |  90° fwd  |      1 |    1 |
| Ballista (shot)    | 12 (3d8)      | 100/420 | Ammunition, loading |   1/3 rnd |  90° fwd  |      1 |    1 |
| Ballista (chain)   | 12 (3d8)      |  60/200 | Ammunition, loading |   1/3 rnd |  90° fwd  |      1 |    1 |
| Stinger            |  8 (2d8)      | 100/400 | Ammunition, loading |   1/1 rnd |     360°  |      1 |    1 |
| Trebuchet \*       | 32 (8d8)      | 300/900 | Ammunition, loading |   1/5 rnd |   5° fwd  |      4 |    6 |
| Fire Thrower       |  4 (1d8)/rnd  |  50/150 | Ammunition, special |   1/2 rnd |  45° fwd  |      2 |    3 |
| Smoke Projector    |               |  30' r  | Ammunition          |   1/4 rnd |        - |      2 |    3 |  

\* Indirect-fire weapons cannot target anything within a 60 ft. radius and can have no overhead obstruction

* Shot does full damage to hull and half damage to rigging
* Chain does full damage to rigging and personnel and half damage to hull

### Naval Tactics

#### Board

In order to board an opposing ship, the helmsman must first close with it or ram it. Once two ships are within boarding range (10 feet), characters can either attempt to leap from one ship to the other with a successful Strength(Athletics) check (DC 10) or by laying boarding planks across the gap.

Ships two or more size categories apart are assumed to have sufficiently disparate deck heights that characters cannot use boarding planks or jump from the lower ship to the higher ship. However, those on the lower ship may use grappling hooks to attempt to climb on board (a ranged attack against AC 10 to secure the grapple, followed by a Strength(Athletics) check with a DC of 10).

A boarding plank is simply a large board, approximately 15 feet long and 3 feet wide. At least one character is required to hold the boarding plank in place, and up to three people can hold one plank. Enemies can attempt to dislodge boarding planks by winning an opposed Strength check against the character(s) securing the plank. Crossing the boarding plank requires a Dexterity(Acrobatics) check (DC 12).

Characters can also attempt to board by swinging from the rigging of one ship onto the other. This requires at least a Strength(Athletics) check of DC 15. On a failure, the character must succeed on a Strength(Athletics) check at DC 10 or fall (either into the water, or onto the deck of one of the ships). Success on the second check indicates that the character manages to safely swing back to the rigging of the original ship.

#### Broadside

A broadside involves sailing a course directly parallel to the opposing ship (traveling either in the same direction or in the opposite direction). This maneuver is so that, as the attacking ship comes alongside the enemy, it can fire all of the weapons mounted on one side of the ship at nearly point blank range.

Initiating a broadside requires no skill check. A broadside maneuver is a move action, and does not include any attacks.

#### Close

The attacking ship maneuvers in close enough to allow troops to board the enemy. In order to initiate a close maneuver, a ship must have enough movement remaining in the round to move adjacent to the enemy’s ship and be able to turn onto a parallel course. If these prerequisites are met, the helmsman can attempt to close. Closing requires a Profession (sailor) check at DC 20.

Success indicates that the ship has pulled alongside the enemy, avoiding the hazards associated with close sailing, and is now within 10 feet of the enemy ship. Each round, the helmsman matches the enemy’s speed and maneuvers automatically (within the limits of his ship’s capabilities, of course) unless the enemy successfully performs an Evade maneuver (detailed below).

Failing the close check by a margin of 4 or less indicates that the helmsman failed to initiate the maneuver correctly; the ship suffers all the normal risks of close sailing. If the check is failed by a margin of 5 or more, however, the ships strike as if the helmsman had initiated a ram maneuver.

Closing is a move action.

#### Evade

When an enemy ship has closed, the helmsman can attempt an evade maneuver to break away from the enemy. An evade maneuver requires a Profession (sailor) check with a DC equal to the result of the Profession (sailor) check that initiated the Close maneuver.

A success indicates that the ship has broken away successfully. The helmsman can then immediately take a second move action to maneuver away from the enemy ship. A failed check by a margin of 4 or less indicates that the helmsman merely failed to break away from the enemy. If the check is failed by 5 or more, however, the helmsman has “zigged when he should have zagged” and collided with the enemy ship. Treat this as a ram maneuver that only deals 1/2 normal damage, since the ships merely sideswipe instead of colliding head-on.

Evading is a full-round action.

#### Fend Off

The fend off maneuver is used once an enemy ship has closed with and grappled the ship. The helmsman can not only attempt to jostle the enemy’s boarding hooks loose, but he can make it risky for an enemy crew to attempt to board.

A fend off maneuver requires a Profession (sailor) check with a DC of 15 + 2 for every three boarding hooks set. Success indicates that the helmsman dislodged 1d3 of the enemy’s boarding hooks +1d3 for every 5 points by which the he beat the DC. Any enemy attempting to board when the fend off maneuver is executed suffers a +2 modifier to the DC of whatever skill check is required to board (Jump checks for characters leaping aboard, Balance checks for those using boarding planks).

The Fend Off maneuver is a move action.

#### Fire

Fire deals damage as usual for the source of the fire, except that ships do not get a Dexterity save to avoid damage.

However, fire attacks deal half damage (divide the damage dealt by 2 before applying the damage threshold) the first round and each subsequent round. The fire continues until it is extinguished.

A fire can be extinguished by covering the area with water, sand, wet tarps and so on. A character needs 2 gallons of water or sand (or a wet tarp of appropriate size), as well as a Dexterity check (DC 15) to extinguish a single 5-foot section of hull or rigging.

#### Grapple

After a successful close maneuver, a captain can order the crew to set boarding hooks and effectively grapple the enemy’s ship (grapnels or boarding hooks are considered standard equipment for any ship intending to engage in combat). At least three members of the crew must make successful attack rolls against at least three separate sections of an enemy ship’s hull (normally, when a boarding action is imminent, crewmen ready actions to set grapples). If successful, the enemy vessel is ensnared and unable to break away until its helmsman can successfully initiate a fend off maneuver and dislodge all the hooks. Grapple maneuvers are usually employed immediately before boarding.

Grappling is a standard action.

#### Out Boats

A desperate maneuver used by sail-powered ships in calm winds, outing boats involves putting two or more of the ship’s launches in the water and using them to tow the ship. If two launches are used to tow the ship, they can move the ship at a speed of 5 feet. Four launches can move the ship at a speed of 10 feet, and eight launches can move it at a speed of 15 feet. In all cases, the ship’s maneuverability is Clumsy while using this maneuver.

#### Overrun

Provided a ship has moved at least 10 feet during the last round, it can attempt to overrun another ship. This is an opposed check using the ship’s Seaworthiness to calculate a bonus as though it were Strength. On a success, the attacking ship moves through the space of the other ship, which loses its next movement. On a failure, the attacking ship stops and loses its next movement. Regardless of the outcome, both ships take damage equal to half the damage they would have taken in a ram (see below).

Passing Through is a standard action.

#### Rake

A rake works like a broadside maneuver, except that the ship sails perpendicular to the enemy, firing across its bow or stern. Rakes are safer than broadsides because most ships have much less weapon coverage to fore and aft than they do from port to starboard. A stern rake also has a major advantage in that the captain’s traditional place on a ship is the quarterdeck at the stern of the ship. Skilled archers in a stern rake can often incapacitate or even kill the captain, which can severely hamper the crew’s morale and fighting spirit. While bow rakes are less likely to kill a senior officer, they still have the advantage of avoiding most of the enemy’s firepower.

Using the rake maneuver is a move action, and does not include any attacks.

#### Ram

To initiate a ram, the helmsman needs only to contact the enemy ship with his own ship. When the ships collide, the attacking ship deals the ram damage listed per 10 feet of movement relative to the other ship.

Ramming a ship is a full-round action.


#### Reef the Sails

Reefing the Sail” entails partially furling the sails to gain maneuverability in close combat at the cost of speed. A ship with reefed sails loses 10 feet of its speed (to a minimum speed of 5 feet), but its maneuverability increases by one category.

A ship’s maneuverability rating can go no higher than “good,” even with reefed sails. A ship with Good maneuverability and reefed sails gains no bonus to maneuverability, but still loses 10 feet of its sail speed.

Reefing the sails takes the same time as to change sail by one level.

#### Tacking

No ship can sail directly into the wind without magical assistance. A ship that attempts to sail directly into the wind "luffs" (stops moving) and loses the rest of its movement for the round. The next round, the helmsman may take a full-round action to turn the ship up to 45°, allowing it to move again.

Ships wishing to sail upwind must use a tactic called “tacking”. Tacking requires taking a zigzag course as close to directly into the wind as possible. A proa-rigged outrigger "shunts" while tacking (the bow becomes the stern and vice-versa). Tacking requires the helmsman make a Profession (sailor) check DC 15. On a failure, the ship luffs as described above.

#### Wet the Sails

Wetting the sails is a standard practice before going into battle. Crewmen dump buckets of seawater on the sails, thoroughly soaking them. While this adversely affects the sails’ ability to catch the wind, it makes them much more resistant to fire attacks. Wetting the sails reduces a ship’s speed by 10%, but it grants the rigging resistance to fire. It takes 10 minutes to wet the sails, and the effects last for about an hour.

# References

[Rob Ossian's Pirate Cove](http://www.thepirateking.com/index.htm)