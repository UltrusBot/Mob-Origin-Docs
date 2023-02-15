# Modify Villager Reputation
This power type allows you to effectively modify the reputation of a villager when you interact with it.

You can learn more about reputation [here](https://minecraft.fandom.com/wiki/Villager#Gossiping).


### Fields
Field | Type | Default | Description
------|------|---------|-------------
bientity_condition | [Bi-entity Condition Type](https://origins.readthedocs.io/en/latest/types/bientity_condition_types/) | *optional* | This is a bi-entity condtion with the actor, the player, and the target, the villager.
modifier | [Attribute Modifier](https://origins.readthedocs.io/en/latest/types/data_types/attribute_modifier/) | *optional* | This is a modifier that will be applied to your reputation with the villager.
modifiers | [List of Modifier Types](https://origins.readthedocs.io/en/latest/types/data_types/attribute_modifier/) | *optional* | This is a list of modifiers that will be applied to your reputation with the villager.


### Example
```json
{
  "type": "moborigins:modify_villager_reputation",
  "modifier": {
    "operation": "addition",
    "value": 100.0
  }
}
```
This power massively increases your reputation with villagers, allowing you to trade with them for much cheaper.
