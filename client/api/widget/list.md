## list

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| __section_header_height | number/function | |
| __section_header_data | function | |
| __section_footer_height | number / function | |
| __section_footer_data | function | |
| __row_height | number / function | |
| __row_data | function | |
| __row_layout | function | |
| __row_count | number / function | |
| __index_titles | function | |
| __title_index | function | |
| __section_count | number / function | |
| dragDownLayout | layout | |
| dragDownMinMovement | number | |
| onDragDownStateChanged | function | |
| onDragDownAction | function | |
| onselected | function | |

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |

### lua sample
```lua
-- section range 0-MAX, row range 0-MAX

list.__row_count = 100
-- or
list.__row_count = function(list, section)
    return section * 3 -- row count by section in list
end

list.__row_height = 60
-- or
list.__row_height = function(list, section, row)
    return 60 -- row height by section&row in list
end

local selectedMap = {}
list.__row_data = function(list, section, row)
    local item = {
        title = {text = selectedMap[section .. "_" .. row] and "selected" or "not selected"},
        btn = {
            onclick = function()
                if selectedMap[section .. "_" .. row] then
                    selectedMap[section .. "_" .. row] = false
                else
                    selectedMap[section .. "_" .. row] = true
                end
                list:reload(section, row) -- reload row by section&row
            end}
    }
    return item
end
list.__section_count = 3
list:reload()
```
