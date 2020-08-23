 
# Age of Empires Game Design: 
Of course proper GDDs would be a collaboration of several game designers and updated over the iterations by a whole development team, but this would be a first draft to start from, add and improve upon. 
 
## UI Wireframe 
As an exercise I created a quick wireframe sketch of the main in game UI.

<img src="/AoE/Aoe2Wireframe.png" alt="UI Wireframe" width="600"/> 

## Small tweaks
Changes implementable in a reasonably short time, but aimed to still have a noticeable positive impact on gameplay.

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
 

## Civ additions
Some possible civ choices I found while researching european groups and cultures. Since 20 AoE 2 civilizations are already actors in the european/mediterranean region, all the most famous groups active in the middle ages are obviously already implemented, or have some overlap with an already implemented one. 

I specifically did game design examples for Venice at the bottom, the others are just civ choices based on history, grouped to fit into a theme that makes sense and is not totally unknown in pop culture.



### West Francia (after fall of the Franks, time of viking warrior Rollo)
- Kingdom of France

- Normany/Normans

- Burgundy

- potentially some group out of the germanic stew of dukes and kingdoms, Bavaria, Bohemia, old swiss confederacy, Saxons, Flanders/Flemish, etc.


### Nordic Migration
A possible expansion theme would be the vikings who left Scandinavia and became distinct groups with their own history and culture. 
Already kind of implemented in the Vikings civ, but since they were not one homogenous culture we can differentiate the existing Vikings civ from those who settled outside of Scandinavia.


#### Normans
French, christian vikings, mostly from denmark, who were part of the Kingdom of France for some time, but also invaded Spain, Britain,  and northern Italy (Byzantium at the time).

Well known in modern culture due to their impact on the history of France, England and the rest of Europe.

#### Lombards
Southern Scandinavians (or potentially only northern germanic) who made it through the middle of europe down to northern Italy after the Gothic Wars had depopulated it and raided and ruled there
Lost northern Italy to the franks 774 and southern Italy to the Normans in the 11th century. Name originates either from their long beards or their Odin-worship
Less well known than the Normans, but we already have a map named after their empire so AoE players usually have at least heard of it.

#### Varangians/Rus'
Viking merchants, mercenaries, pirates and settlers who lived above the black sea and along the volga. Ruled Eastern Europe/Russia as the Kievan Rus' before the Mongol/Tatar invasion

Varangian Guard is famous as the elite Byzantian army mercenaries and bodyguard for the Byzantine emperor. This would already be an easy Unique Unit choice, they should then also be unconvertible, since they were known for their loyalty.

#### Icelandic
If a fourth civ is desired in line with previous expansions, something from the Iceland/Greenland/Norway vikings could be chosen.

They would likely be less known in pop culture than the others, but as we can see in this image around 900 AD, there seems to have been a northwestern language/culture distinct from the others. And there would be plenty of icelandic sagas to use for inspirations.

<img src="/AoE/Old_norse,_ca_900.png" alt="Old Norse" width="400"/> 
https://en.wikipedia.org/wiki/File:Old_norse,_ca_900.PNG

### Geographical alternative
If we want the civs to have met in the same region in a relevant manner, we have Northern Italy for the Normans, Lombards and Varangians (as part of the Byzantine Empire). 

If we want a fourth civ in the area, replacing Iceland with Venice could be a (non-viking) choice.

### Republic of Venice
Most likely founded by people fleeing the germanic and hun invasion and raids, part of the Byzantine Empire, but defending themselves against the Lombards as the Duchy of Venetia.

Gained power through trade, politics and maritime warfare almost exclusively.

They have some overlap with italians, especially with the silk road trading bonus, but Pisa, Genoa and everyone other actor in the "The Ambrosian Republic" campaign is still Italian.

They were active throughout the middle ages and dealt with Byzantines, Franks, Slavs, Saracens, Lombards, Arabs, Normans, Genovese, Ottomans and more, therefore their place in Age of Empires 2 would be well deserved

#### Facts that can inspire mechanics:

- stole relics (repeatedly)

- wealth through trade

- had slaves (and went to war with the church over it)

- got a cut of the plunder of constantinople (and stole some more relics, maybe their unique unit should be able to carry relics)

- Marco Polo (exploration bonus, maybe line of sight on ships as civ bonus)


#### Boni
Team bonus: +2 line of sight on ships 

Civ bonus: Relics also grant wood (as a bonus to their navy aswell)

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

Healing building/field hospital/"Lazarett". Like a hut/tent with 5-10 garrison space and 6-10x healing speed (Like herbal medicine), could also stack with herbal medicine, (additive to 12x, not multiplicative)

Should be able to garrison cavalry, like castles, since healing other units is barely used by top players.

Should probably only be unlocked in castle age, since healing mass scouts or MAA could be too strong in feudal rushes.

Should be quick to destroy, as it provides easy cover for any army and while the enemy is destroying the building, the army hiding inside it can heal back up. So it should be visually displayed as a tent, with about the durability of a palisade wall.

Would need a civ that has some high hitpoint unit as one of its go to strats, elephants or knights at least.
 

Consequences: could benefit tower rushes (if available in feudal) and other strategies involving forward buildings, could make a strong monkless knight siege push

Cost suggestion: 100 wood 20 gold, higher cost than a house and at minimum a small gold cost so it doesnt get too spammed if a lategame player has 5k wood


#### Unique siege weapon:

<img src="/AoE/espringal.png" alt="Espringal" width="300"/> 


A ballista shooting siege unit that assembles like a trebuchet, "Springald" was a medieval version of the roman scorpion that could be used by a european civ.
 
This ["springald catapult"](https://www.youtube.com/watch?v=vIinZrWERUE) version even looks like a trebuchet for bolts.

<img src="/AoE/espringal2.png" alt="Espringal 2" width="300"/> 

- higher range than scorpions

- good in defense 

- could also deal more bonus damage to buildings than scorpion bolts

It could also feature a less than 360 degree shooting angle after setting up, if that provides interesting gameplay, but that would require a lot more design work. 

Since it is mentioned in De Re Militari, most fitting to Byzantium and other civs inheriting Roman military technology, like the Italians, Venice or Franks. https://en.wikipedia.org/wiki/De_re_militari

