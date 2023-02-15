# Action On Entity Tame
This power type allows you to run a bi-entity action when you tame a mob, on the tamer (Actor) and the tamed mob (Target).


### Fields
Field | Type | Default | Description
------|------|---------|-------------
bientity_action | [Bi-entity Action Type](https://origins.readthedocs.io/en/latest/types/bientity_action_types/) | *optional* | This is a bi-entity action with the actor, the player, and the target, the animal you tamed.
bientity_condition | [Bi-entity Condition Type](https://origins.readthedocs.io/en/latest/types/bientity_condition_types/) | *optional* | This is a bi-entity condtion with the actor, the player, and the target, the animal you tamed.


### Example
```json
{
  "type": "moborigins:action_on_entity_tame",
  "bientity_condition": {
    "type": "origins:target_condition",
    "condition": {
      "type": "origins:entity_type",
      "entity_type": "minecraft:cat"
    }
  },
  "bientity_action": {
    "type": "origins:target_action",
    "action": {
      "type": "origins:explode",
      "power": 10
    }
  }
}
```
This power will make it so when you tame a cat, it explodes.
