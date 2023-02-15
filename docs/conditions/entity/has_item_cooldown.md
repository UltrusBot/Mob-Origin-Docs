# Has Item Cooldown
Checks if the player has an item cooldown.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
item | Item | *Optional* | The item to set the cooldown of.
hand | Hand | *Optional* | The hand to check for an item to set the cooldown of, if set, will ignore the item parameter. Valid values are `MAIN_HAND` and `OFF_HAND`.


### Example
```json
{
    "type": "moborigins:has_item_cooldown",
    "item": "minecraft:iron_sword"
}
```
Checks if the player has an item cooldown for iron swords.
