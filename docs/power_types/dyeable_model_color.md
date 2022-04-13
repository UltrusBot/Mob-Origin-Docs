# Dyeable Model Color 
!!! tip "Version Added: 2.0.0"

    This was added in Mob Origins 2.0.0, so it won't work in older versions.
[Power Type](../power_types.md)

This power type acts similarly to the origins [Model Color Power](https://origins.readthedocs.io/en/latest/types/power_types/model_color/), but with the additional feature of being able to dynamically change the color through the [Consume Dye Color](../actions/entity/consume_dye_color.md) entity action.

### Fields


Field  | Type | Default | Description
-------|------|---------|-------------
red | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float) | `1.0` | Default red value for color, Range of: [0.0 - 1.0].
green | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float) | `1.0` | Default green value for color, Range of: [0.0 - 1.0].
blue | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float) | `1.0` | Default blue value for color, Range of: [0.0 - 1.0].
alpha | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float) | `1.0` | Alpha value for color, Range of: [0.0 - 1.0]

### Example

```json
{
    "type": "moborigins:dyeable_model_color",
    "red": 1.0,
    "green": 0.5,
    "blue": 0,
}
```
This power makes you orange.