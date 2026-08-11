# MacLib

my attempt to remakea Mac lib

## Loadstring Setup

```lua
local MacLib = loadstring(game:HttpGet("[https://raw.githubusercontent.com/Springtrappy/Maclib-Repo/refs/heads/main/main-src](https://raw.githubusercontent.com/Springtrappy/Maclib-Repo/refs/heads/main/main-src)"))()

-- Toggle Element
MacLib:CreateToggle("Enable Feature", function(state)
    print("Toggle State:", state)
end)

-- Button Element
MacLib:CreateButton("Click Me", function()
    print("Button clicked!")
end)

-- Slider Element
MacLib:CreateSlider("WalkSpeed", 16, 200, 16, function(value)
    print("Slider Value:", value)
end)

-- Dropdown Element
MacLib:CreateDropdown("Select Team", {"Red", "Blue", "Green"}, "Red", function(selected)
    print("Selected Option:", selected)
end)

-- Color Picker Element
MacLib:CreateColorpicker("Theme Color", Color3.fromRGB(255, 0, 0), function(color)
    print("Selected Color:", color)
end)

-- Textbox Element
MacLib:CreateTextbox("Custom Value", "Type here...", function(text)
    print("Typed Text:", text)
end)

-- Label Element
MacLib:CreateLabel("Static Text Label")
