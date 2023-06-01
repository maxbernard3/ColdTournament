# Game

This document is to be used as a place to write down what the game is too be. It'll be updated as idea get precised and technical decision are made.

## Gameplay Loop

### inspiration
Something in the style of [Cold War Trumpament](https://apkpure.com/cold-war-trumpament/sbm.trump.free) /!\ have addblock or turn off JS before clicking. 
Tweaked to fix the deficiencies I have found from playing the game. feature would added later to deepen the gameplay. the fix list of tweak :
1. limit the strategy consiting of bombing the enemy factory early in the game snowbaling into the victim being incapable of producing new aircraft to stop his factory from being bombed
  a. make factory have more HP
  b. prevent factory destruction 2 cicle back to back
  c. alow for factory size increase, ofering a tradeoff between survivability and force concentration
2. changing the game objective to colecting a target number of points to both encourage the players to focus on fighting for point and reduce the time for a full game from 1-4h down to 20-100min
3. make technology mater more in dice roll to make old aircraft spam as interceptor less viable
4. make aircraft have more ressell value to allow for more meaningfull economy decision
5. base airbase have less room, and are cheaper, allow for airbase upgrade. allow for choice between dispertion increasing survivability or concentration allowing for mass attack and defensse
6. hide enemy force composition (but not number), make defenders decision more dificult than just matching enemy quality and number
7. **(temporary)** both side play the same country to avoid one side stomping the other with unbalanced technologycal advantage (would eventualy let the player have control of RnD to make technology choice)

### Game loop
The game loop would look like that :
- A turn to buildup and organize 
  - in this phase one of the player would ready itself to attack while the other would ready it's defense. 
  - they can purchase new aircraft, bases, factory
    - Base take one cicle to build and cost procurment points
    - Factory take one cicle to build
    - a factory can be upgraded with cp once to increase production number at the cost of hp
    - base can be upgraded with cp to hold either more small aircraft or more heavy aircraft (the later also increase small aircraft capacity to a lesser extent)
  - aircraft are made in factory and cost procurment points
    - it takes one cicle to build aircraft
    - if the factory is damaged it stop production for one turn
    - if the factory is destroyed it stop production for one cicle
    - a factory can build half as many big aircraft as it can small one
    - you can sell aircraft for a PP profit. the more modern the aircraft the greater the profit, at the cost of increassed upfront cost
  - they can move the aircraft around to make the defense easier
    - airbase have limited capacity
    - larger aircrafts take more space 
    - an attack can only be launched with the aircraft from one airbase at a time
    - defense can only be launched with the aircraft from one airbase at a time
    - if an airbase was bombed it may not be capable of operating larger aircraft when the attack turn is on
    - if an airbase was completly destroyed no aircraft can be launched on the attacking turn
  - if any building (exept target) was damaged it heals a partialy
- A combat turn
  - Enemy will send wave of plane with either bomber or defense mission
  - bomber mission will strike at pre selected target
  - target can be :
    1. Point objective, once destroyed will count toward the target score
    2. Airbase, if an airbase is destroyed during an attack it can no longer contribute to the defense
    3. Factory, can't be destroyed twice in a row   
  - defense mission will try to defend bomber mission from enemy
  - defender can send it's own aircrafts to intercept
    - two aircraft meeting will have a roll dice to decide victor
    - roll dice can be tilted depending on which aircraft is more advanced and more suited for the situation
    - the roll can be either :
      1. a draw, interceptor and attacker will be out of the fight
      2. a win, winer can keep fighting
      3. a lose, loser is out of the fight or as a chance to be destroyed. destroyed probablility depend on technology disadventage. attacker is proportinonaly more likely to get destroyed.
    - The encounter end when either side is out of fighting aircraft
  - if attacker win, the bomber that are weren't put out of the fight can bomb target, damage on target depend of technology
  - attacker can send an other wave of attack, the aircraft alredy used by either side on this turn are unavailable for the rest of the turn, regardless of combat roll output
  - turn end when attacker want to stop or is out of aircraft
- An other buildup turn to organise around the damage sustained
- A combat turn with reversed rolls
- At the end of the 2nd combat turn you get:
  - a fixed amount of PP & CP
  - unlock new aircraft (only on certain turn)
  - new target are genarated to replace the destroyed one

The game end when either player reach the target score.

#### defining term
Procurment Point (PP): point awarded at the end of each cicle used to purchase aircraft and bases 
Construction Point (CP): awarded at the end of each cicle, used to make and upgrade factory. can also upgrade base
Cicle : buildup turn, defence turn, buildup turn, attack turn



