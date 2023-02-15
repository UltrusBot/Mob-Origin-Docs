# In Raid Area
This condition checks if the entity is in a raid area.



### Example
```json
{
    "type": "origins:conditioned_attribute",
    "modifier": {
        "attribute": "minecraft:generic.attack_damage",
        "operation": "addition",
        "value": 2.0,
        "name": "Increased damage in raid"
    },
    "tick_rate": 20,
    "condition": {
        "type": "moborigins:in_raid_area"
    }
}
```
This power will increase the player's attack damage by 2.0 while in a raid.
