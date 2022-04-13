# Dyeable Model Color 

[Entity Action](../../entity_actions.md)

This action consumes the currently held dye item, and blends the color of the [Dyeable Model Color Powers](../../power_types/dyeable_model_color.md) with the dye color.

!!! tip "Version Added: 2.0.0"

    
### Fields
*None*

### Example

```json
{
    "type": "origins:active_self",
    "entity_action": {
        "type": "moborigins:consume_dye"
    },
    "cooldown": 1,
    "hud_render": {
        "should_render": false
    },
    "key": {
        "key": "key.use",
        "continuous": true
    },  
}
```
This power absorbs the currently held dye when you right click.