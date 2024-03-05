local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/therealzeek/cat/main/README.lua"))()

local Window = Library:CreateWindow("unison.cc", Vector2.new(398, 310), Enum.KeyCode.P)

local AimingTab = Window:CreateTab("main")

local testSection = AimingTab:CreateSector("main", "left")

testSection:AddTextbox("Prediction", nil, function(State)
    -- Add functionality here if needed
end)

testSection:AddButton("Enable", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/SmfE8e9c'))()
end)

local miscTab = Window:CreateTab("msc")

local miscSection = miscTab:CreateSector("misc", "left")

miscSection:AddButton("rightclick", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/BalligusapoTT/BalligusapoTT/main/Leftclickballi'))()
end)

miscSection:AddButton("qtool", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/RgWV4UFv'))()
end)

local ToggleBind = miscSection:AddToggle("Keybind w/Toggle", false, function(isEnabled)
    -- Add functionality here if needed
    if isEnabled then
        print("Toggle enabled")
    else
        print("Toggle disabled")
    end
end)

ToggleBind:AddKeybind()

AimingTab:CreateConfigSystem("right")

loadstring(game:HttpGet("https://raw.githubusercontent.com/therealzeek/unison.cc/main/README.lua", true))()
