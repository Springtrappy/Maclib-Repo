# MacLib

Clean, lightweight, and responsive Roblox UI library designed with smooth animations and dynamic sizing.

## Script Usage

```lua
local MacLib = loadstring(game:HttpGet("[https://raw.githubusercontent.com/Springtrappy/Maclib-Repo/refs/heads/main/main-src](https://raw.githubusercontent.com/Springtrappy/Maclib-Repo/refs/heads/main/main-src)"))()

MacLib:CreateToggle("Enable Feature", function(state)
    print("Toggle:", state)
end)

MacLib:CreateButton("Click Me", function()
    print("Button pressed")
end)

MacLib:CreateSlider("WalkSpeed", 16, 100, 16, function(val)
    print("Slider:", val)
end)

MacLib:CreateDropdown("Select Mode", {"Mode A", "Mode B", "Mode C"}, "Mode A", function(selected)
    print("Dropdown:", selected)
end)

MacLib:CreateColorpicker("UI Theme", Color3.fromRGB(255, 0, 0), function(color)
    print("Color:", color)
end)

MacLib:CreateTextbox("Input Text", "Type here...", function(text)
    print("Textbox:", text)
end)

MacLib:CreateLabel("Simple Label")
