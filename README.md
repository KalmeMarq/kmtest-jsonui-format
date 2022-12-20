# KM Json UI Format (Testing)

I plan to make a JsonUI mod for Minecraft Java and this repo is for me to put files with the format that I'm currently testing.

The format that Bugrock uses it's complicated to parse and a big mess so I want to make my own and add more unique features too. 

## New Controls/Properties

### `stack_panel`

- gap
  	- type: `integer`
    - description: `Gap between the stack children`

### `pressable_label`

- text
  - type: `string`
  - description: `Renders when element is not being hovered`

- hover_text
  - type: `string`
  - description: `Renders when element is being hovered`

### `custom[panorama_renderer]`

- use_global_time
  - type: `boolean`
  - description: `If it should use a global timer. If two screens have a panorama, by default each have an internal timer so it will start at 0. With use_global_time enabled they will always be synced together`

### `custom[splash_text_renderer]`

- rotation
  - type: `integer`
  - description: `Rotation in the z-axis. Uses degrees`

- speed
  - type: `float`
  - description: `Speed of the scaling`
  
## SubProperties

If, for example, an element has always 20px of height and you just want to be changing the width, then you can use the width property. Subproperties have higher priority than the respective full property.
 
### `size`
  - width
  - height
  
### `max_size`
  - max_width
  - max_height
  
### `min_size`
  - min_width
  - min_height
  
### `anchor`
  - anchor_from
  - anchor_to
  
### `offset`
  - offset_x
  - offset_y
  
### `uv`
  - u
  - v
 
### `uv_size`
  - u_width
  - v_height
  
### `nineslice_size`
  - nineslice_left
  - nineslice_right
  - nineslice_top
  - nineslice_bottom

### `gap`
  - column_gap
  - row_gap
