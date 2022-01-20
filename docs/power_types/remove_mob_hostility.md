# Remove Mob Hostility

[Power Type](../power_types.md)

This power allows you to remove the hostility of certain mobs. It's limited to certain mobs which have the TargetGoal goal type. This means entities with brains (Piglins, Hoglins, and Villagers) won't be affected by this power.

### Fields

Field | Type | Default | Description
------|------|---------|-------------
`entity_condition` | [Entity Condition](https://origins.readthedocs.io/en/latest/types/entity_condition_types/) | *Optional* | This is a condition for the entity you wish to make neutral.
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
This power will make it so creatures in the undead entity group are neutral towards you.