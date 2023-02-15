# Fog
Changes the fog color of the entity.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
red | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) |   | The red value of the fog color.
green | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) |   | The green value of the fog color.
blue | [Float](https://origins.readthedocs.io/en/latest/types/data_types/float/) |   | The blue value of the fog color.
start | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) |   | The start distance of the fog.
end | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) |   | The end distance of the fog.


### Example
```json
{
  "type": "moborigins:fog",
  "red": 1,
  "green": 1,
  "blue": 1,
  "start": -1,
  "end": 30,
  "condition": {
    "type": "apoli:sneaking",
    "inverted": true
  }
}
```
This makes it so the player has a thick white fog, which can be disabled by sneaking.

This looks like:

![Fog Image](../images/fog.png)
