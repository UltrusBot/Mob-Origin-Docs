# Set Dyeable Model Color
Sets the color of the entity's Dyeable Model Color Power, if it has one.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
red | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) | *1.0* | The red value of the color to set the DyeableModelColorPower to.
green | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) | *1.0* | The green value of the color to set the DyeableModelColorPower to.
blue | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) | *1.0* | The blue value of the color to set the DyeableModelColorPower to.


### Example
```json
{
    "type": "origins:action_over_time",
    "duration": 100,
    "entity_action": {
        "type": "origins:if_else",
        "condition": {
             "type": "origins:daytime"
        },
        "if_action": {
            "type": "moborigins:set_dyeable_model_color",
            "red": 1.0,
            "green": 1.0,
            "blue": 1.0
        },
        "else_action": {
            "type": "moborigins:set_dyeable_model_color",
            "red": 10.0,
            "green": 0.0,
            "blue": 0.0
        }
    }
 }
```
At night, the entity will be red. During the day, the entity will be white.
