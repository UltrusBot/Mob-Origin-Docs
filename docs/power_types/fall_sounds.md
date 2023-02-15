# Fall Sounds
Changes the entity's fall sounds.


### Fields
Field | Type | Default | Description
------|------|---------|-------------
distance | [int](https://origins.readthedocs.io/en/latest/types/data_types/integer/) | *4* | The distance the entity must fall to play the big fall sound.
small_fall_sound | [sound_event](https://origins.readthedocs.io/en/latest/types/data_types/sound_event/) | *entity.generic.small_fall* | The sound to play when the entity falls a small distance.
big_fall_sound | [sound_event](https://origins.readthedocs.io/en/latest/types/data_types/sound_event/) | *entity.generic.big_fall* | The sound to play when the entity falls a big distance.


### Example
```json
{
  "type": "moborigins:fall_sounds",
  "big_fall_sound": "minecraft:entity.slime.squish",
  "small_fall_sound": "minecraft:entity.slime.squish_small"
}
```
Changes the entity's fall sounds to the slimes squish sounds.
