Certainly! Here's the README with the section added at the top:

### Library 

```lua
local uilibrary = loadstring(game:HttpGet("https://raw.githubusercontent.com/Kiet1308/tvkhub/main/rac"))()
```

### Window 

```lua
local windowz = uilibrary:CreateWindow("Syrex Hub", "Pet Simulator 99", true)
```

```lua
local Section1 = Page1:CreateSection("Section Name")
```

### Section Example

```lua
local Section1 = Page1:CreateSection("Section Name")
```

#### Slider Example
```lua
Page1:CreateSlider("Slider Example", {Min = 16, Max = 500, DefaultValue = 30}, function(Value)
   print(Value)
end)
```

#### Toggle Example
```lua
Page1:CreateToggle("Toggle Example", {Toggled=false , Description = false}, function(Value)
   print(Value)
end)
```

#### Button Example
```lua
Page1:CreateButton("Button Example", function ()
   print("Button Clicked!")
end)
```

#### Textbox Example
```lua
Page1:CreateTextbox("TextBox", false, function (Value)
   print(Value)
end)
```

#### Dropdown Example
```lua
Page1:CreateDropdown("Dropdown ", {
   List = {"Value1", "Value2", "Value3", "Value4"},
   Default = "None"}, function(value)
       print(value)
end)
```

#### Color Picker Example
```lua
Page1:CreateColorPicker("Color Picker", Color3.fromRGB(255, 255, 255), function ()
   print("Color Selected")
end)
```

#### Refresh Dropdown Example
```lua
local dropdown = Page1:CreateDropdown("Refresh Dropdown ", {
   List = {"Value1", "Value2", "Value3", "Value4"},
   Default = "None"}, function(value)
       print(value)
end)
```
