# Mimic Enchant
Mimics an enchantment on the entity, acting as if the entity had the enchantment, while not actually having it.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
enchantment | [Enchantment](https://origins.readthedocs.io/en/latest/types/data_types/enchantment/) |   | The enchantment to mimic.
level | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) |   | The level of the enchantment to mimic.


### Example
```json
{
  "type": "moborigins:mimic_enchant",
  "enchantment": "minecraft:frost_walker",
  "level": 3
}
```
Mimics the Frost Walker enchantment on the entity.

 ### Extra Info



This will also change the result of the `origins:enchantment` entity condition.



This doesn't work on all enchantments due to limitations in minecraft. These are the ones that do work:

 - All Protection Enchantments

 - Sweeping Edge

 - Knockback

 - Fire Aspect

 - Respiration

 - Depth Strider

 - Efficiency

 - Looting

 - Aqua Affinity

 - Frost Walker

 - Soul Speed

 - Power

 - Punch

 - Flame
