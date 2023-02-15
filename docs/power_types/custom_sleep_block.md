# Custom Sleep Block
This power type allows you to sleep on blocks other than beds.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
block_condition | [Block Condition Type](https://origins.readthedocs.io/en/latest/types/block_condition_types/) | *optional* | This determines what type of block you can sleep on, if null, any block will work.


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
This power will make it so that you can sleep on any log block.
