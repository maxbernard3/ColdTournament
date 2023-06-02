# Game

This document is to be used as a place to write down what the game is to be. It'll be updated as ideas get precise and technical decisions are made.

## Gameplay Loop

### Inspiration
Something in the style of [Cold War Trumpament](https://apkpure.com/cold-war-trumpament/sbm.trump.free) /!\ Have Adblock or turn off JS before clicking. 
Tweaked to fix the deficiencies I have found from playing the game. Features would be added later to deepen the gameplay. The fix list of tweaks:
1. Limit the strategy consisting of bombing the enemy factory early in the game snowballing into the victim being incapable of producing new aircraft to stop his factory from being bombed.
    a. Make factory have more HP.
    b. Prevent factory destruction 2 cycles back to back.
    c. Allow for factory size increase, offering a tradeoff between survivability and force concentration.
2. Change the game objective to collecting a target number of points to both encourage the players to focus on fighting for points and reduce the time for a full game from 1-4h down to 20-100min.
3. Make technology matter more in dice roll to make old aircraft spam as interceptors less viable.
4. Make aircraft have more resale value to allow for more meaningful economy decisions.
5. Base airbases have less room and are cheaper, allow for airbase upgrade. Allow for choice between dispersion, increasing survivability, or concentration, allowing for mass attack and defense.
6. Hide enemy force composition (but not number), making defender's decision more difficult than just matching enemy quality and number.
7. **(Temporary)** Both sides play the same country to avoid one side stomping the other with an unbalanced technological advantage (would eventually let the player have control of R&D to make technology choices).

### Game Loop
The game loop would look like this:
- A turn to build up and organize 
  - In this phase, one of the players would ready itself to attack while the other would ready its defense.
  - They can purchase new aircraft, bases, and factories.
    - Bases take one cycle to build and cost procurement points.
    - Factories take one cycle to build.
    - A factory can be upgraded with BP once to increase production numbers at the cost of HP.
    - Base can be upgraded with BP to hold either more small aircraft or more heavy aircraft (the latter also increases small aircraft capacity to a lesser extent).
  - Aircraft are made in the factory and cost procurement points.
    - It takes one cycle to build aircraft.
    - If the factory is damaged, it stops production for one turn.
    - If the factory is destroyed, it stops production for one cycle.
    - A factory can build half as many big aircraft as it can small ones.
    - You can sell aircraft for a PP profit. The more modern the aircraft, the greater the profit, at the cost of increased upfront cost.
  - They can move the aircraft around to make the defense easier.
    - Airbases have limited capacity.
    - Larger aircraft take more space.
    - An attack can only be launched with the aircraft from one airbase at a time.
    - Defense can only be launched with the aircraft from one airbase at a time.
    - If an airbase was bombed, it may not be capable of operating larger aircraft when the attack turn is on.
    - If an airbase was completely destroyed, no aircraft can be launched on the attacking turn.
  - If any building (except the target) was damaged, it heals partially.
- A combat turn
  - The enemy will send waves of planes with either bomber or defense mission.
  - Bomber missions will strike at a pre-selected target.
  - The target can be:
    1. Point objective, once destroyed, will count toward the target score.
    2. Airbase, if an airbase is destroyed during an attack, it can no longer contribute to the defense.
    3. Factory, can't be destroyed twice in a row.
  - Defense missions will try to defend bomber missions from the enemy.
  - The defender can send its own aircraft to intercept.
    - Two aircraft meeting will have a dice roll to decide the victor.
    - The dice roll can be tilted depending on which aircraft is more advanced and more suited for the situation.
    - The roll can be either:
      1. A draw, interceptor and attacker will be out of the fight.
      2. A win, the winner can keep fighting.
      3. A loss, the loser is out of the fight or has a chance to be destroyed. The probability of being destroyed depends on the technological disadvantage. The attacker is proportionally more likely to get destroyed.
    - The encounter ends when either side is out of fighting aircraft.
  - If the attacker wins, the bombers that weren't put out of the fight can bomb the target. The damage to the target depends on technology.
  - The attacker can send another wave of attack. The aircraft already used by either side on this turn are unavailable for the rest of the turn, regardless of the combat roll output.
  - The turn ends when the attacker wants to stop or is out of aircraft.
- Another buildup turn to organize around the damage sustained.
- A combat turn with reversed rolls.
- At the end of the 2nd combat turn, you get:
  - A fixed amount of PP & BP.
  - Unlock new aircraft (only on certain turns).
  - New targets are generated to replace the destroyed ones.

The game ends when either player reaches the target score.

#### Defining Terms
**Procurement Point (PP):** Points awarded at the end of each cycle used to purchase aircraft and bases. <br>
**Building Point (BP):** Points awarded at the end of each cycle, used to make and upgrade factories. Can also upgrade bases. <br>
**Cycle:** Buildup turn, defense turn, buildup turn, attack turn. <br>




