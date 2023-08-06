local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Lazzy Hub", HidePremium = false, IntroText = "Lazzy Hub", SaveConfig = true, ConfigFolder = "Lazzy Hub"})

OrionLib:MakeNotification({
    Name = "Thank",
    Content = "Cam on vi da dung scrip",
    Image = "rbxassetid://4483345998",
    Time = 5
})

local MainTab = Window:MakeTab({
    Name = "Home",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

local Section = MainTab:AddSection({
    Name = "Lazzy Hub Menu"
})


MainTab:AddButton({
    Name = "Button!",
    Callback = function()
              print("Lazzy Hub")
      end    
})

MainTab:AddToggle({
    Name = "Toggle",
    Default = false,
    Callback = function(Value)
        print("Lazzy Hub")
    end    
})

MainTab:AddColorpicker({
    Name = "Colorpicker",
    Default = Color3.fromRGB(255, 0, 0),
    Callback = function(Value)
        print(Value)
    end      
})

MainTab:AddSlider({
    Name = "Slider",
    Min = 0,
    Max = 20,
    Default = 5,
    Color = Color3.fromRGB(255,255,255),
    Increment = 1,
    ValueName = "bananas",
    Callback = function(Value)
        print(Value)
    end    
})

OrionLib:Init()
