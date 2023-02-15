# Illuminate
This power type allows you to make a mob emit light like a glow squid.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
light | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) | *15* | The light level the mob will emit.


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
