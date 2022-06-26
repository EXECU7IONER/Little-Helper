--Rebirth Champions X - Coconut Farm GUI
-- 
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local Title = Instance.new("TextLabel")
local TextLabel = Instance.new("TextLabel")
local FarmButton = Instance.new("TextButton")
local UICorner = Instance.new("UICorner")
local destryGui = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Frame.BackgroundTransparency = 0.300
Frame.Position = UDim2.new(0.233796299, 0, 0.260553122, 0)
Frame.Size = UDim2.new(0, 180, 0, 90)

Title.Name = "Title"
Title.Parent = Frame
Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Title.BackgroundTransparency = 1.000
Title.Position = UDim2.new(0.027777778, 0, 0, 0)
Title.Size = UDim2.new(0, 169, 0, 19)
Title.Font = Enum.Font.SourceSansBold
Title.Text = "Rebirth Champions X"
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.TextScaled = true
Title.TextSize = 14.000
Title.TextWrapped = true

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.Position = UDim2.new(0.027777778, 0, 0.311111122, 0)
TextLabel.Size = UDim2.new(0, 115, 0, 19)
TextLabel.Font = Enum.Font.SourceSansBold
TextLabel.Text = "Coconut Farm"
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

FarmButton.Name = "FarmButton"
FarmButton.Parent = Frame
FarmButton.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
FarmButton.Position = UDim2.new(0.677777767, 0, 0.322222233, 0)
FarmButton.Size = UDim2.new(0, 52, 0, 19)
FarmButton.Font = Enum.Font.SourceSansBold
FarmButton.Text = "OFF"
FarmButton.TextColor3 = Color3.fromRGB(255, 255, 255)
FarmButton.TextScaled = true
FarmButton.TextSize = 14.000
FarmButton.TextWrapped = true

UICorner.CornerRadius = UDim.new(0, 4)
UICorner.Parent = FarmButton

destryGui.Name = "destryGui"
destryGui.Parent = Frame
destryGui.BackgroundColor3 = Color3.fromRGB(255, 85, 0)
destryGui.Position = UDim2.new(0.027777778, 0, 0.74444443, 0)
destryGui.Size = UDim2.new(0, 169, 0, 16)
destryGui.Font = Enum.Font.SourceSansBold
destryGui.Text = "DESTROY GUI"
destryGui.TextColor3 = Color3.fromRGB(255, 255, 255)
destryGui.TextScaled = true
destryGui.TextSize = 14.000
destryGui.TextWrapped = true

UICorner_2.CornerRadius = UDim.new(0, 4)
UICorner_2.Parent = destryGui

local function IZOWCOX_fake_script() -- FarmButton.LocalScript 
	local script = Instance.new('LocalScript', FarmButton)

	wait(2)
	local button = script.Parent.Parent.FarmButton
	local label = script.Parent
	local plr = game.Players.LocalPlayer
	local playerr = game.Players.LocalPlayer.Character.HumanoidRootPart
	
	_G.Toggle = false -- true it collects false it doesnt, re-execute every time you change
	_G.Timer = 60
	
	local function farm()
		if _G.Toggle == true then
			while wait(_G.Timer) and _G.Toggle do -- wait for coconut respawn
				for _,v in pairs(game:GetService("Workspace").Scripts.CoconutsFolder.Storage:GetDescendants()) do
					if v.Name == "TouchInterest" then
						firetouchinterest(playerr, v.Parent, 0)
						firetouchinterest(playerr, v.Parent, 1)
					end
				end
			end
		else
			while wait(_G.Timer) and _G.Toggle do -- wait for coconut respawn
				for _,v in pairs(game:GetService("Workspace").Scripts.CoconutsFolder.Storage:GetDescendants()) do
					if v.Name == "TouchInterest" then
						firetouchinterest(playerr, v.Parent, 0)
						firetouchinterest(playerr, v.Parent, 1)
					end
				end
			end
		end
	end
	
	
	local function toggle()
		if button.BackgroundColor3 == Color3.fromRGB(170, 0, 0) then
			--script to do
			button.BackgroundColor3 = Color3.fromRGB(0, 170, 0)
			button.Text = "ON"
			_G.Toggle = true
			farm()
		else
		if button.BackgroundColor3 == Color3.fromRGB(0, 170, 0) then
			--script to do
			button.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
			button.Text = "OFF"
			_G.Toggle = false
			farm()
		end
		end
	end
	
	button.MouseButton1Down:Connect(function()
		toggle()
	end)
	
end
coroutine.wrap(IZOWCOX_fake_script)()
local function NEMLLED_fake_script() -- destryGui.LocalScript 
	local script = Instance.new('LocalScript', destryGui)

	local frame = script.Parent.Parent.Parent.Frame
	local button = script.Parent.Parent.destryGui
	
	local function destroy()
		frame:Destroy()
	end
	
	
	button.MouseButton1Down:Connect(function()
		destroy()
	end)
end
coroutine.wrap(NEMLLED_fake_script)()
local function QNOGQW_fake_script() -- Frame.LocalScript 
	local script = Instance.new('LocalScript', Frame)

	local frame = script.Parent.Parent.Frame
	frame.Active = true
	frame.Draggable = true
end
coroutine.wrap(QNOGQW_fake_script)()
