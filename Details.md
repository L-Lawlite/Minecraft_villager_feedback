While most of the changes suggested are good and provide more balanced gameplay some of the changes are questionable.I have listed them down below with the ways that can be imporoved based on my opinion.

- Villager from different biome providing different kind of enchantments
  - **Problem with this** - Transporting villager is already a big task even if it is a small distance adding this change will require you to transport them accross multiple biome which is nerf to villager trading to extreme. This will make players discorage to setup villager trade and with lack of easy to get enchantments there will be more rage quits due to loss of items which is already a problem in small to medium size server.
  - **Proposed Solution** - Introduce a way to transport villagers more easily accross multiple biomes.

- Villagers not providing max level enchantment.
  - **Problem with this** - This requires combining of enchantments in the anvil which leads to increase the level cost and make items too expensive to enchant.
  - **Proposed Solution** - Either make the villagers give max level enchantment that are frequently used in almost all items. Like unbreaking, efficiency, protection (maybe) or remove the experience limit from the anvil combining.



Also i would like to have a way to restore the trades back to old system in servers in case servers want to do that without depending on external mods. Since minecraft is all about the way you want to play. For that i have a few suggestions as well.
- Make a gamerule `/gamerule zombieConversionDiscountCount` which is default set to 1 but could have a `infinite` option to make so we can restore the old functionality if we choose.
- Make json formated files to define villager trades and maybe wandering traders too so it can be edited in datapacks. They could be formed as shown below 

      📂 datapacks
        📂 <data_pack>
           📜 pack.mcmeta
           📂 data
             📂 <namespace>
               📂 gameplay
                 📂 villager_trade
                   📂 common
                     📄 armorer.json
                   📂 plains
                     📄 librarian.json
                   📂 swamp
                     📄 librarian.json


In common folder we can include all the trades that are common. If not specified in the biome specific folder game will use this to generate the trades. If specified in biome specific folder plains villager will use trade specified in plains folder. Same can be done with wandering trader and even wandering trader can be made to offer different product based on the biome they spawn in. If chooses to be implemented later.

Now the details about the format of trade files are attached

In this all items are formated as that of a loot table this also allows to have a set of items to be rolled like different set of logs if that trade need to be added also allows full nbt support that is present today as well. The first set of rolls in trades define how many trades need to be unlocked with level up. This roles cant be duplicated so you cant roll u set of same trades from same pools. But can if it is in multiple pools is same as we have right now. This json file is also attached with this. Thank you for reading this big feedback.