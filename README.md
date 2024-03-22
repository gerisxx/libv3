# Library 

```lua
local uilibrary = loadstring(game:HttpGet("https://raw.githubusercontent.com/Kiet1308/tvkhub/main/rac"))()
```

### Window 

```lua
local windowz = uilibrary:CreateWindow("Syrex Hub", "Pet Simulator 99", true)
```

### Section Example 

```lua
local Section1 = Page1:CreateSection("Section Name")
```

#### Slider Example
```lua
-- Slider Example
Section1:CreateSlider(
    "Slider Example", 
    {Min = 16, Max = 500, DefaultValue = 30}, 
    function(Value)
        print(Value)
    end
)
```

#### Toggle Example
```lua
-- Toggle Example
Section1:CreateToggle(
    "Toggle Example", 
    {Toggled = false, Description = false}, 
    function(Value)
        print(Value)
    end
)
```

#### Button Example
```lua
-- Button Example
Section1:CreateButton(
    "Button Example", 
    function ()
        print("Button Clicked!")
    end
)
```

#### Textbox Example
```lua
-- Textbox Example
Section1:CreateTextbox(
    "TextBox", 
    false, 
    function (Value)
        print(Value)
    end
)
```

#### Dropdown Example
```lua
-- Dropdown Example
Section1:CreateDropdown(
    "Dropdown ", 
    {
        List = {"Value1", "Value2", "Value3", "Value4"},
        Default = "None"
    }, 
    function(value)
        print(value)
    end
)
```

#### Color Picker Example
```lua
-- Color Picker Example
Section1:CreateColorPicker(
    "Color Picker", 
    Color3.fromRGB(255, 255, 255), 
    function ()
        print("Color Selected")
    end
)
```

#### Refresh Dropdown Example
```lua
-- Refresh Dropdown Example
local dropdown = Section1:CreateDropdown(
    "Refresh Dropdown ", 
    {
        List = {"Value1", "Value2", "Value3", "Value4"},
        Default = "None"
    }, 
    function(value)
        print(value)
    end
)

-- Refresh Example Button
Section1:CreateButton(
    "Refresh Example", 
    function ()
        local newlist = {"resf", "uwua", "fsk"}
        dropdown:Clear()
        wait(1)
        dropdown:Add(newlist)
    end
)
```
