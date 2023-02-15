# Grow Block
Grows a block if it is fertilizable.



### Example
```json
{
  "type": "apoli:action_on_block_use",
  "block_condition": {
    "type": "apoli:block",
    "block": "minecraft:carrots"
  },
  "block_action": {
    "type": "moborigins:grow"
  }
}
```
This power will grow carrots when right clicked.
