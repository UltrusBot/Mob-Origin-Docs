# Custom Sleep Block 
[Power Type](../power_types.md)

This power type allows you to make it so the player can sleep at blocks other than a bed. 

!!! tip "Version Added: 2.0.0"

    
### Fields

Field | Type | Default | Description
------|------|---------|-------------
block_condition | [Block Condition](https://origins.readthedocs.io/en/latest/types/block_condition_types/) |  | The condition checked against for the custom sleep block.

### Example

```json
{
  "type": "moborigins:custom_sleep_block",
  "block_condition": {
    "type": "origins:in_tag",
    "tag": "minecraft:logs"
  }
}
```
This power allows you to sleep on logs.