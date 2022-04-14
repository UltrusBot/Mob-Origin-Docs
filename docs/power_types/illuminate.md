# Illuminate 
[Power Type](../power_types.md)

This power type allows you to make the entity with the power glow similarly to the glow squid.

!!! tip "Version Added: 2.0.0"

    
### Fields

Field | Type | Default | Description
------|------|---------|-------------
light | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) | `15` | This is the light level. It is clamped to the [0-15] range

### Example

```json
{
    "type": "moborigins:illuminate",
    "light": 15,
    "condition": {
        "type": "origins:exposed_to_sun",
        "inverted": true
    }
}
```
This power makes it so when you are not exposed to the sun (eg: in a cave, or at night) you glow just like a glow squid.