# Modify Attack Distance Scaling Factor
Modifies the distance in which mobs will begin to attack the player.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
bientity_condition | [bientity_condition](https://origins.readthedocs.io/en/latest/types/bientity_condition_types/) |   | A bi-entity condition with the actor, the mob, and the target, the player.
modifier | [modifier](https://origins.readthedocs.io/en/latest/types/data_types/attribute_modifier/) |   | The modifier to apply to the scaling factor.
modifiers | [List of Modifier Types](https://origins.readthedocs.io/en/latest/types/data_types/attribute_modifier/) |   | A list of modifiers to apply to the scaling factor.


### Example
```json
{
  "type": "moborigins:modify_attack_distance_scale",
  "modifier": {
    "operation": "multiply_total",
    "value": -1
  },
  "bientity_condition": {
    "type": "origins:actor_condition",
    "condition": {
      "type": "origins:in_tag",
      "tag": "minecraft:raiders"
    }
  }
}
```
Makes it so raiders are peaceful towards the player, but will attack them if the player attacks them first.
