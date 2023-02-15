# Decrement Cauldron Fluid
Decrements the fluid level of a cauldron.



### Example
```json
{
  "type": "apoli:action_on_block_use",
  "block_condition": {
    "type": "apoli:block",
    "block": "minecraft:water_cauldron"
  },
  "block_action": {
    "type": "moborigins:decrement_cauldron_fluid"
  },
  "entity_action": {
    "type": "moborigins:set_dyeable_model_color",
    "red": 1.0,
    "green": 1.0,
    "blue": 1.0
  }
}
```
This power will make it so when you click on a water cauldron, it will decrement the fluid level and reset your dyeable model color to white.
