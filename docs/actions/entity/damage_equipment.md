# Damage Equipment
Damages an entity's equipment at a specified slot by a specified amount.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
equipment_slot | [EquipmentSlot](https://origins.readthedocs.io/en/latest/types/data_types/string/) |   | The equipment slot to damage, options are: `"mainhand"`, `"offhand"`, `"head"`, `"chest"`, `"legs"`, `"feet"`
amount | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) |   | The amount of damage to deal to the equipment.


### Example
```json
{
  "type": "apoli:action_over_time",
  "entity_action": {
    "type": "moborigins:damage_equipment",
    "equipment_slot": "head",
    "amount": 1
  },
  "interval": 40,
  "condition": {
    "type": "apoli:exposed_to_sun"
  }
}
```
Damages the entity's helmet slot item by 1 every 2 seconds while they are exposed to the sun.
