local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

OrionLib:MakeNotification({
	Name = "Scriptkakmak",
	Content = "Scriptkakmak",
	Image = "rbxassetid://4483345998",
	Time = 5
})

local Window = OrionLib:MakeWindow({Name = "Scriptkakmak", HidePremium = false, SaveConfig = true, ConfigFolder = "Orion"})

--Player Tab--

local PlayerTab = Window:MakeTab({
	Name = "Genaral",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local PlayerSection = PlayerTab:AddSection({
	Name = "RaceV4"
})

PlayerSection:AddButton({
	Name = "Temple of Time",
	Default = false,
	Callback = function()
	        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(28286.35546875, 14895.3017578125, 102.62469482421875)
	        end
	        
})

PlayerSection:AddButton({
	Name = "Mink Door",
	Default = false,
	Callback = function()
	        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(29015.3691, 14890.6582, -379.076508, -0.00146599161, 1.28161051e-10, -0.999998927, 9.37944655e-14, 1, 1.28161051e-10, 0.999998927, 9.23705556e-14, -0.00146599161)
	        end
	        
})

PlayerSection:AddButton({
	Name = "AutoRace",
	Default = false,
	Callback = function()
	        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.MinkTrial.Ceiling.CFrame * CFrame.new(0,-5,0)
	        end
})

--Player Tab End--

--Settings Tab--

local SettingsTab = Window:MakeTab({
	Name = "Settings",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local SettingsSection = SettingsTab:AddSection({
	Name = "Settings"
})

SettingsSection:AddButton({
	Name = "Destroy UI",
	Callback = function()
        OrionLib:Destroy()
  	end    
})

--Settings End--

OrionLib:Init() --UI Lib End
