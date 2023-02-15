# Nearby Entities
Compare the amount of nearby entities based on a given condition.

!!! tip "The 'actor' entity is the entity with the power, while the 'target' entity is the entity that is being checked."


### Fields
Field | Type | Default | Description
------|------|---------|-------------
multiplier | [Double](https://origins.readthedocs.io/en/latest/types/data_types/float/) |   | The factor by which the checking hitbox is multiplied by, with the starting value being your player hitbox.
comparison | [Comparison](https://origins.readthedocs.io/en/latest/types/data_types/comparison/) |   | The comparison to use.
compare_to | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) |   | The value to compare to.
bientity_condition | [BiEntityCondition](https://origins.readthedocs.io/en/latest/types/bientity_condition_types/) | *null* | The condition to check the nearby entities with.


### Example
```json
{
  "type": "origins:self_glow",
  "use_teams": false,
  "red": 1,
  "green": 0,
  "blue": 0,
  "condition": {
    "type": "moborigins:nearby_entities",
    "multiplier": 3,
    "comparison": ">=",
    "compare_to": 3,
    "bientity_condition": {
      "type": "origins:target_condition",
      "condition": {
        "type": "origins:entity_group",
        "group": "undead"
      }
    }
  }
}
```
Makes the entity glow red if there are 3 or more undead entities within 3 blocks of it.
