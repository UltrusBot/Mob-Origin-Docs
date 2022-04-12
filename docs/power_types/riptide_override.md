# Riptide Override

[Power Type](../power_types.md)

This power allows you to change the conditions necessary to use riptide on a trident. 

The original conditions will still work (Water & Rain).
### Fields

Field | Type | Default | Description
------|------|---------|-------------
damage | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) | 1 | The damage applied to the trident after using the power riptide.

### Example

```json
{
   "type":"moborigins:riptide_override",
   "condition":{
      "type":"origins:submerged_in",
      "fluid":"minecraft:lava"
   }
   
}
```
This example will allow you to use tridents while in lava.