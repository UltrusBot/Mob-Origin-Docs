# Time Since Rest
Checks how long the player has been sleeping, time is in ticks.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
comparison | [Comparison](https://origins.readthedocs.io/en/latest/types/data_types/comparison/) |   | The comparison to use.
compare_to | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) |   | The value to compare to.


### Example
```json
{
        "entity_condition": {
            "type": "moborigins:time_since_rest",
            "comparison": "greater_than",
            "compare_to": 100
        }
    }
```
Checks how long the player has been sleeping.
