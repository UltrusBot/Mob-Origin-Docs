# Add Experience to Resource
This power type adds experience points to a resource when collected by the player through an experience orb.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
resource | [Identifier](https://origins.readthedocs.io/en/latest/types/data_types/identifier/) |   | The resource to add experience to


### Example
```json
{
  "type": "apoli:multiple",
  "energy": {
    "type": "origins:resource",
    "min": 0,
    "max": 100,
    "hud_render": {
      "sprite_location": "origins:textures/gui/community/spiderkolo/resource_bar_01.png",
      "bar_index": 3
    }
  },
  "exp": {
    "type": "moborigins:add_experience_to_resource",
    "resource": "*:*_energy"
  }
}
```
Defines a resource, and adds xp to it.
