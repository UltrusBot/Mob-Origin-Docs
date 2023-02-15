# Remove Mob Hostility
This power allows you to remove the hostility of certain mobs. It's limited to certain mobs which have the TargetGoal goal type. This means entities with brains (Piglins, Hoglins, and Villagers) won't be affected by this power.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
entity_condition | [entity_condition](https://origins.readthedocs.io/en/latest/types/entity_condition_types/) |   | The condition that the mob must meet to be affected by this power.


### Example
```json
{
    "type": "moborigins:remove_mob_hostility",
    "entity_condition": {
        "type": "origins:entity_group",
        "group": "undead"
    }
}
```
Removes the hostility of undead mobs towards the player.
