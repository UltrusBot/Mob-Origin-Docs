# Channeling Override
Allows using the channeling enchantment without having the enchantment, and allows you to specify an action to be performed on the trident thrower or the entity hit by the lightning bolt.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
entity_action | [Entity Action](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | *optional* | The action to be performed on the trident thrower.
hit_entity_action | [Entity Action](https://origins.readthedocs.io/en/latest/types/entity_action_types/) | *optional* | The action to be performed on the entity hit by the lightning bolt.


### Example
```json
{
  "type": "moborigins:channeling_override",
  "entity_action": {
    "type": "origins:explode",
    "power": 4
  },
  "hit_entity_action": {
    "type": "origins:add_velocity",
    "y": 2
  }
}
```
This power allows using the channeling enchantment without having the enchantment, and causes the trident thrower to explode and the entity hit by the lightning bolt to be launched into the air.
