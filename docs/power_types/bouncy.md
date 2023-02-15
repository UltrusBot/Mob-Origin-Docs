# Bouncy
Makes the entity bounce off the ground when it lands.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
multiplier | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) | *optional* | The multiplier to apply to the entity's velocity when it lands.


### Example
```json
{
    "type": "moborigins:bouncy",
    "multiplier": -1.00
}
```
This makes the entity bounce off the ground when it lands, without losing any velocity.
