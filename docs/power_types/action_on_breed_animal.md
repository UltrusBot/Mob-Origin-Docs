# Action on Breed Animal

[Power Type](../power_types.md)

This power type allows you to run a bi-entity action when you breed a mob.

### Fields

Field | Type | Default | Description
------|------|---------|-------------
bientity_action | [Bi-entity Action Type](https://origins.readthedocs.io/en/latest/types/bientity_action_types/) | _optional_ | This is a bi-entity action with the actor, the player, and the target, the animal you breed last.
bientity_condition | [Bi-entity Condition Type](https://origins.readthedocs.io/en/latest/types/bientity_condition_types/) | _optional_ | This is a bi-entity condtion with the actor, the player, and the target, the animal you breed last.


```json
{
  "type": "moborigins:action_on_entity_tame",
  "bientity_condition": {
    "type": "origins:target_condition",
    "condition": {
      "type": "origins:entity_type",
      "entity_type": "minecraft:pig"
    }
  },
  "bientity_action": {
    "type": "origins:target_action",
    "action": {
       "type": "origins:spawn_entity",
       "entity_type": "minecraft:pig",
       "tag": "{Age:-24000}"
    }
  }
}
```
This power will make it so when you breed two pigs, another baby pig spawns.