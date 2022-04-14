# Fog 

[Power Type](../power_types.md)

This power lets the entity with the power have a boss bar that shows its health. This also has more fields than you usually access via the /boss bar command.

!!! tip "Version Added: 2.0.0"

    
### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
color | [Boss Bar Color](/docs/data_types/boss_bar_color.md) | `white` | Color of boss bar. 
style | [Boss Bar Style](/docs/data_types/boss_bar_style.md) | `progress` | Style of boss bar. 
darkenSky | [Boolean](https://origins.readthedocs.io/en/latest/types/data_types/boolean/) | `false` | Sets whether the sky will be darkened when the boss bar is visible
thickenFog | [Boolean](https://origins.readthedocs.io/en/latest/types/data_types/boolean/) | `false` | Sets whether the fog will be thickened when the boss bar is visible
text | [Text](https://origins.readthedocs.io/en/latest/types/data_types/string/) | `Entity Name` | Sets the title of the boss bar. Will default to the entity name if left blank.

### Example

```json
{
  "type": "moborigins:health_boss_bar",
  "color": "red",
  "style": "notched_6",
  "darkenSky": "true",
  "thickenFog": "true"
}
```
This creates a red boss bar, with the notched_6 style. It also darkens the sky when you are nearby, and thickens the fog.