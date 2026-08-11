# MacLib

Clean, lightweight, and responsive Roblox UI library designed with smooth animations and dynamic sizing.

```lua
-- Bootstrapping the UI Library
local MacLib = loadstring(game:HttpGet("[https://raw.githubusercontent.com/Springtrappy/Maclib-Repo/refs/heads/main/main-src](https://raw.githubusercontent.com/Springtrappy/Maclib-Repo/refs/heads/main/main-src)"))()

-- Toggle Component
-- Creates an interactive on/off switch returning a boolean state
MacLib:CreateToggle("Enable Feature", function(state)
    print("Toggle State:", state)
end)

-- Button Component
-- Standard action button triggering a custom function on click
MacLib:CreateButton("Click Me", function()
    print("Button clicked!")
end)

-- Slider Component
-- Smooth draggable bar with a knob, live value readout, min/max bounds, and default setting
MacLib:CreateSlider("WalkSpeed", 16, 200, 16, function(value)
    print("Slider Value:", value)
end)

-- Dropdown Component
-- Collapsible list menu for selecting items from an array
MacLib:CreateDropdown("Select Team", {"Red", "Blue", "Green"}, "Red", function(selected)
    print("Selected Option:", selected)
end)

-- Color Picker Component
-- Pop-out window featuring full Hue and Saturation gradient controls
MacLib:CreateColorpicker("Theme Color", Color3.fromRGB(255, 0, 0), function(color)
    print("Selected Color:", color)
end)

-- Textbox Component
-- Text input area returning typed content when focus is lost or enter is pressed
MacLib:CreateTextbox("Custom Value", "Type here...", function(text)
    print("Typed Text:", text)
end)

-- Label Component
-- Display static info text inside your element list
MacLib:CreateLabel("Static Text Label")
