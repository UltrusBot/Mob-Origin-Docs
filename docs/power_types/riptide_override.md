# Riptide Override
Allows using the riptide enchantment without having the enchantment, with a configurable durability cost.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
trident_damage | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) | *optional* | The amount of durability to take from the trident when using the riptide enchantment.


### Example
```json
{
  "type": "moborigins:riptide_override",
  "trident_damage": 10,
  "condition": {
    "type": "origins:daytime",
    "inverted": true
  }
}
```
This allows using the riptide enchantment without having the enchantment, only during the night, at the cost of 10 durability.
