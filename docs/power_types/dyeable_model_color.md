# Dyeable Model Color
Sets the color of a model, while allowing it to be dyed by the [Set Dyeable Model Color](https://moborigins.readthedocs.io/en/latest/actions/entity/set_dyeable_model_color) action, or the [Consume Dye](https://moborigins.readthedocs.io/en/latest/actions/entity/consume_dye_color/) action.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
red | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) | *1.0* | The red component of the color.
green | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) | *1.0* | The green component of the color.
blue | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) | *1.0* | The blue component of the color.
alpha | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) | *1.0* | The alpha component of the color.


### Example
```json
{
    "type": "moborigins:dyeable_model_color",
    "red": 0.0,
    "green": 0.0,
    "blue": 1.0,
    "alpha": 0.9
}
```
Sets the color of a model to blue, and slightly translucent.
