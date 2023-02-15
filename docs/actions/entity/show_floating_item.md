# Show Floating Item
Shows a floating item to the player.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
item_stack | [ItemStack](https://origins.readthedocs.io/en/latest/types/data_types/item_stack/) |   | The item stack to show.


### Example
```json
{
  "type": "origins:action_when_damage_taken",
  "entity_action": {
    "type": "moborigins:show_floating_item",
    "item_stack": {
      "item": "minecraft:creeper_head"
    }
  },
  "cooldown": 1
}
```
Shows a floating creeper head to the player when they take damage.
