# Set Angered At
Sets the target entity to be angered at the actor entity for a specified time. This only works on angerable entities, such as: Endermen, Zombified Piglins, Bees, Iron Golems, Polar Bears, and Wolves.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
time | [int](https://origins.readthedocs.io/en/latest/types/data_types/integer/) | *100* | The time the entity will be angry for.


### Example
```json
{
    "bientity_action": {
        "type": "moborigins:set_angered_at",
        "time": 100
    }
}
```
Sets the entity to be angry at the other entity.
