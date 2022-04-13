# Modify Attack Distance Scale
!!! info "Version Added: 2.0.0

    This was added in Mob Origins 2.0.0, so it won't work in older versions.
[Power Type](../power_types.md)

This power type allows changing the attack distance scale factor that influences the distance certain will see you.

### Fields

Field | Type | Default | Description
------|------|---------|-------------
bientity_condition | [Bi-entity Condition Type](https://origins.readthedocs.io/en/latest/types/bientity_condition_types/) | _optional_ | This is a bi-entity condtion with the actor, the mob, and the target, the player.
modifier | [Attribute Modifier](https://origins.readthedocs.io/en/latest/types/data_types/attribute_modifier) | _optional_ | Modifiers that are applied to attack distance scale factor.
modifiers | [Array](https://origins.readthedocs.io/en/latest/types/data_types/array) of [Attribute Modifiers](https://origins.readthedocs.io/en/latest/types/data_types/attribute_modifier) | _optional_ | Array of modifiers that are applied to attack distance scale factor.

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
      "tag": "minecraft:skeletons"
    }
  }
}
```
This power would make it so you don't get attack by skeletons (unless you stand within the same block as them).