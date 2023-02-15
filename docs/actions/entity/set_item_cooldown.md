# Set Item Cooldown
Sets the cooldown of an item for a player.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
item | Item | *Optional* | The item to set the cooldown of.
ticks | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) | *Required* | The amount of ticks to set the cooldown to.
hand | Hand | *Optional* | The hand to check for an item to set the cooldown of, if set, will ignore the item parameter. Valid values are `MAIN_HAND` and `OFF_HAND`.


### Example
```json
{
    "type": "moborigins:set_item_cooldown",
    "item": "minecraft:shield",
    "ticks": 100
}
```
Sets the cooldown of the shield item to 100 ticks.
