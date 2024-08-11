
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/natoloe009/SCRIPT-ROBLOX/main/Orion%20KaGa.lua')))()
local Window = OrionLib:MakeWindow({Name = "XDAX PIECE BY:เธญเนเธฒเธข เธเธ เธเธ", HidePremium = false, SaveConfig = true, IntroEnabled = false, ConfigFolder = "YourConfig"})

--[[
Name = <string> - The name of the UI.
HidePremium = <bool> - Whether or not the user details shows Premium status or not.
SaveConfig = <bool> - Toggles the config saving in the UI.
ConfigFolder = <string> - The name of the folder where the configs are saved.
IntroEnabled = <bool> - Whether or not to show the intro animation.
IntroText = <string> - Text to show in the intro animation.
IntroIcon = <string> - URL to the image you want to use in the intro animation.
Icon = <string> - URL to the image you want displayed on the window.
CloseCallback = <function> - Function to execute when the window is closed.
]]
local Tab = Window:MakeTab({
	Name = "Mani",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]
local Section = Tab:AddSection({
	Name = "เธเธฑเธเธ•เธดเธ”เธ•เนเธญ:เธญเนเธฒเธข เธเธ เธเธ"
})

--[[
Name = <string> - The name of the section.
]]
Tab:AddButton({
	Name = "เธ•เธตเธ—เธตเน€เธ”เธตเธขเธงเธ•เธฒเธข!",
	Callback = function()
      		local radius = 10
_G.Kill = true
spawn(function()
    while wait() do
        pcall(function()
            if _G.Kill then
              local player = game.Players.LocalPlayer
              local character = player.Character or player.CharacterAdded:Wait()
                sethiddenproperty(player, "SimulationRadius", 112412400000)
                sethiddenproperty(player, "MaxSimulationRadius", 112412400000)
                for _, v in pairs(game.Workspace.mon:GetDescendants()) do
                    if v:IsA("Humanoid") and v.Parent and v.Parent:IsA("Model") then
                        local npcPosition = v.Parent:FindFirstChild("HumanoidRootPart") and v.Parent.HumanoidRootPart.Position
                        local playerPosition = character:FindFirstChild("HumanoidRootPart") and character.HumanoidRootPart.Position
                        if npcPosition and playerPosition and (npcPosition - playerPosition).Magnitude <= radius then
                            if v.Health < v.MaxHealth then
                              wait(.1)
                                v.Health = 0
                            end
                        end
                    end
                end
            end
        end)
    end
end)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
local Tab = Window:MakeTab({
	Name = "TP",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเน€เธเธดเธ”",
	Callback = function()
      		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1269.9187, 36.9980202, 411.331818, -0.998564422, 2.57111168e-08, 0.0535641946, 2.39274769e-08, 1, -3.39403954e-08, -0.0535641946, -3.26100142e-08, -0.998564422)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเน€เธซเนเธ”เน€เน€เธ”เธ",
	Callback = function()
      	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1229.73083, 28.1940842, -909.99115, -0.993344724, 3.85920558e-08, 0.115179323, 4.33531042e-08, 1, 3.88309225e-08, -0.115179323, 4.35658727e-08, -0.993344724)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเธฅเธญเธขเธเนเธฒ",
	Callback = function()
      		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-341.123169, 210.047684, 665.151611, 0.977458715, -7.3529236e-09, -0.211126521, -2.50056753e-09, 1, -4.64040468e-08, 0.211126521, 4.58859759e-08, 0.977458715)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเธกเธฒเธขเธเธฒเธ",
	Callback = function()
      		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-943.880371, 39.4492683, 1523.11987, -0.0229947548, 5.4626323e-08, 0.999735594, 6.03331074e-08, 1, -5.32530606e-08, -0.999735594, 5.90926135e-08, -0.0229947548)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐPVP",
	Callback = function()
      		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-883.898193, 46.8670692, -170.284561, -0.961327314, 0, 0.275408566, 0, 1.00000012, -0, -0.275408566, 0, -0.961327314)
  	end    
})
--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเน€เธ—เธเน€เธเธฒ",
	Callback = function()
      		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2436.65991, 36.087265, 1053.73279, -0.99991703, 0, -0.012886093, 0, 1.00000012, -0, 0.012886093, -0, -0.99991703)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเธเนเธณเน€เน€เธเนเธ",
	Callback = function()
      		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2410.50171, 28.7867146, 279.253937, 0.0217868779, -1.82997795e-08, -0.999762654, -1.60176441e-08, 1, -1.86531821e-08, 0.999762654, 1.64202376e-08, 0.0217868779)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเธกเธฑเธเธเธฃ",
	Callback = function()
  game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2848.05347, 28.5305691, -74.943634, 0.027035322, 0, -0.999634504, -0, 1, -0, 0.999634504, 0, 0.027035322)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเธชเธธเนเธกเธเธฅ",
	Callback = function()
      		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1837.38135, 28.0941277, -262.412903, -0.829081953, -0, -0.559127152, -0, 1, -0, 0.559127152, 0, -0.829081953)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
Tab:AddButton({
	Name = "เน€เธเธฒเธฐเธกเธญเธเธเธฒเธขเธ”เธฒเธเธเธฒเนเธ”เน",
	Callback = function()
      		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2458.66235, 229.122574, -724.1604, -0.999942005, -4.05037959e-08, 0.0107676983, -4.05463361e-08, 1, -3.73257292e-09, -0.0107676983, -4.16894697e-09, -0.999942005)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]











Tab:AddButton({
	Name = "เธชเธเธดเธเธเธดเธเน€เธเธทเนเธญเนเธกเนเธกเธตเน€เธเธฒเธฐเนเธเธเธตเน",
	Callback = function()
      		loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\40\39\104\116\116\112\115\58\47\47\103\105\115\116\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\109\101\111\122\111\110\101\89\84\47\98\102\48\51\55\100\102\102\57\102\48\97\55\48\48\49\55\51\48\52\100\100\100\54\55\102\100\99\100\51\55\48\47\114\97\119\47\101\49\52\101\55\52\102\52\50\53\98\48\54\48\100\102\53\50\51\51\52\51\99\102\51\48\98\55\56\55\48\55\52\101\98\51\99\53\100\50\47\97\114\99\101\117\115\37\50\53\50\48\120\37\50\53\50\48\102\108\121\37\50\53\50\48\50\37\50\53\50\48\111\98\102\108\117\99\97\116\111\114\39\41\44\116\114\117\101\41\41\40\41\10\10")()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]
