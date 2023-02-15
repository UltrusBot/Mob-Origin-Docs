# Resource Math
This action type allows to do math, from one resource onto another.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
power_type | [Power Type](https://origins.readthedocs.io/en/latest/types/power_types/) | *required* | Left side of the equation, and the resource that stores the result.
math_operator | [Math Operator](/) | *required* | The math operator you want to use. Can be "`add`", "`subtract`", "`multiply`", "`divide`", "`mod`", "`exponent`", or "`set`".
power_type | [Power Type](https://origins.readthedocs.io/en/latest/types/power_types/) | *required* | Right side of the equation, and the resource that stores the value.


### Example
```json
{
  "type": "origins:multiple",
  "resource1": {
    "type": "origins:resource",
    "min": 0,
    "max": 100,
    "start_value": 1,
    "hud_render": {
      "sprite_location": "origins:textures/gui/community/spiderkolo/resource_bar_01.png",
      "bar_index": 2
    }
  },
  "resource2": {
    "type": "origins:resource",
    "min": 0,
    "max": 100,
    "start_value": 1,
    "hud_render": {
      "sprite_location": "origins:textures/gui/community/spiderkolo/resource_bar_01.png",
      "bar_index": 3
    }
  },
  "active1": {
    "type": "origins:active_self",
    "entity_action": {
      "type": "moborigins:resource_math",
      "to_resource": "*:*_resource1",
      "from_resource": "*:*_resource2",
      "operator": "add"
    }
  },
  "active2": {
    "type": "origins:active_self",
    "key": {
      "key": "key.origins.secondary_active"
    },
    "entity_action": {
      "type": "moborigins:resource_math",
      "to_resource": "*:*_resource2",
      "from_resource": "*:*_resource1",
      "operator": "add"
    }
  }
}
```
This power defines two resources, and allows using the primary active to add the value of the secondary resource to the primary resource, and the secondary active to add the value of the primary resource to the secondary resource.
