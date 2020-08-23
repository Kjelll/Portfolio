Link back to [portfolio overview](/README.md).

# Age of Empires Game Design: 
Of course proper GDDs would be a collaboration of several game designers and updated over many iterations by a whole development team, but these snippets would be a first draft to start from, add and improve upon. 
 
## UI Wireframe 
As an exercise I created a quick wireframe sketch of the main in game UI.

<img src="/AoE/Aoe2Wireframe.png" alt="UI Wireframe" width="800"/> 



## Small tweaks
Changes implementable in a reasonably short time, but aimed to still have a noticeable positive impact on gameplay.

### Show resource total for villager groups
Making a group of villagers show the sum of the resources they carry instead just showing nothing.  

Here is a quick example case:

<img src="/AoE/SumRes/Problem_statement.jpg" alt="Problem_statement" width="600"/> 

Desired impact: Players no longer need to individually cycle through their villagers when they need to reach a specific amount of food asap (Villager, Feudal research, Castle research). 
		
Here would be a possible UI example, where the resource is shown like a final entry in the list of selected units.

<img src="/AoE/SumRes/Possible_solution.jpg" alt="possible_solution" width="600"/> 

Issues: Vills carrying different resources. If showing different resources is significantly more demanding to implement, conflicts can be solved by either only showing the highest resource, or none at all. 

Impacted gameplay: Quality of Life change, Eco, Dark age/minimally in Feudal age 

### Making global queue items cancellable
Right clicking on a unit in the global unit queue directly cancels it, instead of requiring players to left click it (at the top left) and then cancel it (in the bottom middle).

Desired impact: Misclicking militia while shift spamming halbs and hussar doesnt force the player to slowly cycle through his barracks to cancel each individually

Issues: Research must be excluded to avoid game losing misclicks (cancelling Imp or Paladin)
<img src="/AoE/SumRes/Issue.jpg" alt="Issue" width="200"/> 

Impacted gameplay: Quality of Life change, Military, Imp/Post Imp

### Cavalry charge sound effect when a big group of cavalry moves towards a big group of enemies
Similar to the charge sound effect already implemented in AoM, but more sparsely triggered and only some slight horse gallop sound to not disturb important sound cues.

Desired impact: Give the player a feeling of power while commanding a group of knights, without disturbing the rest of their gameplay experience

Impacted gameplay: Audio only
 



## Ornamental Buildings
A concept for buildings that serve no gameplay relevant purpose, but have customizable visuals shared across clients. Allowing players to showcase event rewards they earned to others would decisively lift them above the developer-created visual mods that event rewards represent right now.

Introducing (as rewards) the social/community motivators of cosmetics that so many games sell as their main financial income could greatly improve the player retention gained from the frequent event challenges taking place in AoE 2 DE.

### Concept
The easiest implementation would be a granite block that is mechanically worse than a palisade wall in every way, but customisable with a number of different statues, fountains and more in the player profile.

A decent size of base content could be quickly created by gray scaling all units and putting them on a pedestal to create a stone statue of each unit. The same could be repeated but in gold, to create a more rare (and tougher to obtain) version. Some AoE 1 units could be used aswell to create "ancient" statues.

Issues: A part of the nostalgic playerbase absolutely hates how modern games have changed and especially cosmetics are often seen as the downfall of modern video games, therefore they should be kept clearly distinct from modern cosmetics. 
They should stay free (only locked behind challenges) and away from the main gameplay (no unit skins), as those would be red lines to cross.
The name cosmetics should also be avoided, hence the name "ornamental buildings". 
That way any backlash could likely be kept below the level of Autoscout.


#### Variation 1: Single statue
Only one type of statue can be built, only one item has to be added to the villager build menu (one empty space in civil building menu)
The statue visual can only be changed between games, at the start of the game each players statue sprite is initialised as their currently in the profile selected statue.

<img src="/AoE/OrnamentalBuildings/IntegratedCivilBuildingMenu.jpg" alt="Integrated in the civil building menu" width="300"/> 

Issues: "Empty" building menu space conflicts with the Feitoria as Portugese, misclicks between statue and similar hotkeys could annoy players.


#### Variation 2: Multiple Ornamental Buildings
Each player can select up to 13 different skins at the same time, which are then placed in a new villager build menu, which could be located between the repair and garrison options of the "main" villager menu.

This would allow more roleplay- or casual- oriented players to decorate their city with a number of statues, fountains and other trinkets to make their empire pretty to look at.

It would also make it more relevant to own more than one statue for Achiever player types.

<img src="/AoE/OrnamentalBuildings/OrnamentalBuildingMenu.png" alt="Ornamental Building Menu" width="400"/> 

There is plenty of empty space in the main villager menu, even the top row still has a slot for one button, which can then open an Ornamental Building Menu.

<img src="/AoE/OrnamentalBuildings/OrnamentalBuildings.png" alt="Ornamental Buildings" width="400"/> 

Benefits: Adding an extra menu sets them apart from civil and military buildings in the other menus and makes misclick building less likely.

Issues: A full menu for ornamental buildings alone would give them a more prominent position in the villager menu, which could also annoy the hardcore anti-cosmetic playerbase.
The menu button could be moved from the top row to the bottom left to give it a more optional feel.

## Civ additions
For more game design instead of history skip to [Venice](#Venice), the others are just civ choices based on historicity, grouped to fit into a theme that makes sense and is not totally unknown in pop culture.

Some possible civ choices I found while researching european groups and cultures. Since 20 AoE 2 civilizations are already actors in the european/mediterranean region, all the most famous groups active in the middle ages are obviously already implemented, or have some overlap with an already implemented one. 




### West Francia (after fall of the Franks, time of viking warrior Rollo)
- Kingdom of France

- Normany/Normans

- Burgundy

- potentially some group out of the germanic stew of dukes and kingdoms, Bavaria, Bohemia, old swiss confederacy, Saxons, Flanders/Flemish, etc.


### Nordic Migration
A possible expansion theme would be the vikings who left Scandinavia and became distinct groups with their own history and culture. 

Already to some degree implemented as the Vikings civ, but since they were not one homogenous culture we can differentiate the existing Vikings civ from those who settled outside of Scandinavia.


#### Normans
French, christian vikings, mostly from denmark, who were part of the Kingdom of France for some time, but also invaded Spain, Britain,  and northern Italy (Byzantium at the time).

Well known in modern culture due to their impact on the history of France, England and the rest of Europe.

#### Lombards
Southern Scandinavians who migrated through the middle of Europe down to northern Italy after the Gothic Wars had depopulated it and raided and ruled there

Lost northern Italy to the Franks 774 and southern Italy to the Normans in the 11th century. Name originates either from their long beards or their Odin-worship. Either way their unique unit should have a long beard.

Less well known than the Normans, but we already have a map named after their empire so AoE players have at least heard of it.

#### Varangians/Rus'
Viking merchants, mercenaries, pirates and settlers who lived along the volga and the black sea. Ruled Eastern Europe/Russia as the Kievan Rus' before the Mongol/Tatar invasion

Varangian Guard is famous as the elite Byzantian army mercenaries and bodyguard for the Byzantine emperor. This would already be an easy Unique Unit choice, they should then also be unconvertible, since they were known for their loyalty.

#### Icelandic
If a fourth civ is desired in line with previous expansions, some northern viking groups from Iceland/Greenland/Scotland/Norway  could be chosen.

They would likely be less known in the mainstream than the others, but as we can see in this map around 900 AD, there seems to have been a northwestern language/culture distinct from the others. And there would be plenty of Icelandic sagas to use for inspirations.

<img src="/AoE/Old_norse,_ca_900.png" alt="Old Norse" width="400"/> 
https://en.wikipedia.org/wiki/File:Old_norse,_ca_900.PNG

### Geographical alternative
If we want the civs to have met in the same region in a relevant manner, we have Northern Italy for the Normans, Lombards and Varangians (fighting for the Byzantine Empire). 

If we want a fourth civ in the area, replacing Iceland with Venice could be a (non-viking) choice.

### Republic of Venice <a name="Venice"></a>
Most likely founded by people fleeing the germanic and hun invasion and raids, part of the Byzantine Empire at first, defending themselves against the Lombards as the Duchy of Venetia.

Gained power through trade, politics and maritime warfare.

They have some overlap with Italians, especially with the silk road trading bonus, but Pisa, Genoa and everyone other actor in the "The Ambrosian Republic" campaign is still Italian.

They were active throughout the middle ages and dealt with Byzantines, Franks, Slavs, Saracens, Lombards, Arabs, Normans, Genovese, Ottomans and more, so their place in Age of Empires 2 would be well deserved.

#### Facts that can inspire mechanics:

- stole relics (repeatedly)

- wealth through trade

- had slaves (and went to war with the church over it)

- got a cut in the plunder of Constantinople (and stole some more relics, maybe their unique unit should be able to carry relics)

- Marco Polo (exploration bonus, maybe line of sight on ships as civ bonus)


#### Bonuses
Team bonus: +2 line of sight on ships 

Civ bonus: Relics also grant wood (as a bonus to their navy and to incentivise stealing relics)

Civ bonus: Players trading with a Venetian market also grant Venice a (small) portion of their earnings


#### Unique Tech Inspirations:

- [Devotion of Verona](https://en.wikipedia.org/wiki/Devotion_of_Verona_to_Venice) should grant some buff regarding settlements/town centers. Istrian and Dalmation cities also swore allegiance to Venice again in 1000    

- [Marriage of the Sea](https://en.wikipedia.org/wiki/Marriage_of_the_Sea_ceremony) for some maritime bonus, if possible something relating to "the sea may be calm and quiet"


#### Military:

- Strong naval presence, they basically won their empire on water, then lost it on land. Should have a strong ship bonus.

- Crusaders in the fourth crusade were transported by Venice, in return they sieged Zara and later Constantinople. So they should have a decent knight line, at least cavalier, even though only some of the knights sieging Constantinople were Venetian.

Not much else on land until the 15. century, where they had mostly condotierrri armies on land.

- Since their only significant land armies seem to have been condottieri, they should get condotierri like the existing Italians and they also used more specifically [Stradioti](https://en.wikipedia.org/wiki/Military_history_of_the_Republic_of_Venice#XV_century&:~:text=Stradioti), cavalry mercenaries from albania/macedonia, wikipedia about them [here](https://en.wikipedia.org/wiki/Stratioti#Republic_of_Venice_and_Kingdom_of_Naples_(Italy))

- the most impressive fact about their land army is how they managed to lose almost every land battle but still survive through their politics and money. That is hard to recreate in AoE though.



#### Unique Units

- [Stradioti](https://en.wikipedia.org/wiki/Military_history_of_the_Republic_of_Venice#XV_century&:~:text=Stradioti), light cavalry mercenaries (1400-1800), represented as a fast cavalry unit (some mix between hussar and paladin) that costs only gold. Their imperial upgrade also allows them to carry relics. 

Some more venetian unit could come from in depth research of venice land battles, since Stradioti were not from Venice and not exclusively used by Venice, the UU choice is far from perfect.

- Condotierri, not "unique" since the main Italians already have them but clearly should be in the venetian arsenal.

- [Bucentaur](https://en.wikipedia.org/wiki/Bucentaur), a strong "boss battle" unique ship similar to the turtle ship.  


### Unused Ideas

#### Healing Tent/Field Hospital
Best on a civ that was famous for its medicine in some way, like Teutons (who got Herbal Medicine because of it). 

Healing building/field hospital/"Lazarett". A hut/tent with 5-10 garrison space and 6-10x healing speed (Like herbal medicine), could also stack with herbal medicine, (additive to 12x, not multiplicative)

Should be able to garrison cavalry, like castles, since healing other units is barely used by top players.

Should probably only be unlocked in castle age, since healing mass scouts or MAA could be too strong in feudal rushes.

Should be quick to destroy, as it provides easy cover for any army and while the enemy is destroying the building, the army hiding inside it can heal back up. So it should be visually displayed as a tent, with about the durability of a palisade wall.

Would need a civ that has some high hitpoint unit as one of its go to strats, elephants or knights at least.
 

Consequences: could benefit tower rushes (if available in feudal) and other strategies involving forward buildings, could make a strong monkless knight siege push

Cost suggestion: 100 wood 20 gold, higher cost than a house and at minimum a small gold cost so it doesnt get too spammed if a lategame player has 5k wood


#### Unique siege weapon:

<img src="/AoE/espringal.png" alt="Espringal" width="300"/> 


A ballista shooting siege unit that assembles like a trebuchet, the Springald or Espringal was a medieval version of the roman scorpion that could be used by Byzantine or European civs.
 
This ["springald catapult"](https://www.youtube.com/watch?v=vIinZrWERUE) version even looks like a trebuchet for bolts.

<img src="/AoE/espringal2.png" alt="Espringal 2" width="300"/> 

Bad mobility as a tradeoff with higher range and more bonus damage to buildings than scorpion.

Could also feature a less than 360 degree shooting angle after setting up, if that provides interesting gameplay, but that would require a lot more design work. 

Since it is mentioned in De Re Militari, most fitting to Byzantium and other civs inheriting Roman military technology, like the Italians, Venice or Franks. https://en.wikipedia.org/wiki/De_re_militari

