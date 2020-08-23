 
# Age of Empires Game Design: 
Of course proper GDDs would be a collaboration of several game designers and updated over the iterations by a whole development team, but this would be a first draft to start from, add and improve upon. 
 
## Small tweaks
Changes implementable by a single dev, but aimed to still have a noticeable positive impact on gameplay.

### Show resource total for villager groups
Making a group of villagers show the sum of the resources they carry instead just showing nothing.  

Here is a quick example case:

<img src="/AoE/SumRes/Problem_statement.jpg" alt="Problem_statement" width="600"/> 

Desired impact: Players no longer need to individually cycle through their villagers when they need to reach a specific amount of food asap (Villager, Feudal research, Castle research). 
		
Here would be a possible UI example.

<img src="/AoE/SumRes/Possible_solution.jpg" alt="possible_solution" width="600"/> 

Issues: Vills carrying different resources, if showing different resources is technically significantly more demanding, conflicts can be solved by only showing the highest resource, or none at all. 

Impacted gameplay: Quality of Life change, Eco, Dark age/minimally in Feudal age 

### Making global queue items cancellable
Right clicking on something in the global unit queue directly cancels it, instead of requiring players to left click it (at the top left) and then cancel it (in the bottom middle).

Desired impact: Misclicking militia while shift spamming halbs doesnt force the player to slowly cycle through his barracks to cancel each individually

Issues: Research is excluded to avoid game losing misclicks (cancelling Imp or Paladin)

<img src="/AoE/SumRes/Issue.jpg" alt="Issue" width="200"/> 

Impacted gameplay: Quality of Life change, Military, Imp/Post Imp

### Cavalry charge sound effect when a big group of cavalry attack moves towards a big group of enemies
Similar to the charge sound effect already implemented in AoM, but more sparsely triggered and only some slight horse gallop sound to not disturb important sound clues or make the player weary of triggering it every minute.

Desired impact: Give the player a feeling of power while commanding a group of knights, without disturbing the rest of their gameplay experience

Impacted gameplay: Audiovisual

## Extentions and Expansions
Ideas that would add to instead of change the existing game.


### Civ additions
Some possible civ choices I found while researching european groups and cultures. Since 20 AoE 2 civilizations are already actors in the european/mediterranean region, all the most famous groups active in the middle ages are obviously already implemented. 

#### Nordic Migration
A possible expansion theme would be the vikings who left Scandinavia and became distinct groups with their own history and culture. Already kind of implemented in the Vikings civ, but since they were not one homogenous culture we can differentiate the existing Vikings civ as those who only raided and did not settle outside of Scandinavia.


##### Normans
French, christian vikings, mostly from denmark, who were part of the Kingdom of France for some time, but also invaded Spain, Britain,  and northern Italy (Byzantium at the time).
Well known in modern culture
##### Lombards
Vikings who made it through the middle of europe down to northern Italy and raided and ruled there
Less well known than the Normans, but we already have a map named after their empire so AoE players usually have at least heard of it.
##### Varangians/Rus'
Viking merchants, mercenaries, pirates and settlers who lived above the black sea and along the volga. Ruled Eastern Europe/Russia as the Kievan Rus' before the Mongol/Tatar invasion
Varangian Guard is famous as the elite Byzantian army mercenaries and bodyguard for the Byzantine emperor.

##### Icelandic
If a fourth civ is desired in line with previous expansions, something from the Iceland/Greenland/Norway vikings could be chosen, but would likely be less known in pop culture than the others.
But as we can see in this image around 900 AD, there seems to have been a northwestern language/culture distinct from the others.
<img src="/AoE/Old_norse,_ca_900.png" alt="Old Norse" width="500"/> 
https://en.wikipedia.org/wiki/File:Old_norse,_ca_900.PNG


### Limited replay rewind
Since real rewinding  in the replay system/engine is technically too demanding to implement (or impossible), the save state system could be utilized to allow for rewinds save points, if the required memory isnt too great.
So for example each 1, 5 or 10 minutes, the replay creates a backup state like the save and quit backup to restore a lobby match with a disconnect, which the viewer can then revert back to if he wishes to do so.
To better gauge feasibility here is an overview of the required features:
-The replay system needs to initialise at a save state
-Save states must be made from replays
-Replay saves should be made in the background if possible, if a pause and saving animation is necessary, backups every 5, 10, or even more minutes can still be acceptable





 