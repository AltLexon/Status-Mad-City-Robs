-- Status Gui --
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local Frame_2 = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local Jewel = Instance.new("TextLabel")
local Club = Instance.new("TextLabel")
local Casino = Instance.new("TextLabel")
local Bank = Instance.new("TextLabel")
local Pyramid = Instance.new("TextLabel")
local UICorner_2 = Instance.new("UICorner")

--Properties:

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(0, 255, 51)
Frame.BackgroundTransparency = 0.500
Frame.Position = UDim2.new(0.00896495581, 0, 0.569018364, 0)
Frame.Size = UDim2.new(0, 180, 0, 263)

UICorner.Parent = Frame

Frame_2.Parent = Frame
Frame_2.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
Frame_2.BackgroundTransparency = 0.500
Frame_2.BorderSizePixel = 0
Frame_2.Position = UDim2.new(0, 0, 0.106463879, 0)
Frame_2.Size = UDim2.new(0, 180, 0, 2)

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.BorderSizePixel = 0
TextLabel.Size = UDim2.new(0, 180, 0, 28)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "Status"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

Jewel.Name = "Jewel"
Jewel.Parent = Frame
Jewel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Jewel.BackgroundTransparency = 1.000
Jewel.Position = UDim2.new(0, 0, 0.144486696, 0)
Jewel.Size = UDim2.new(0, 180, 0, 33)
Jewel.Font = Enum.Font.SourceSans
Jewel.Text = "Jewel:"
Jewel.TextColor3 = Color3.fromRGB(0, 0, 0)
Jewel.TextScaled = true
Jewel.TextSize = 14.000
Jewel.TextWrapped = true

Club.Name = "Club"
Club.Parent = Frame
Club.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Club.BackgroundTransparency = 1.000
Club.Position = UDim2.new(0, 0, 0.311787069, 0)
Club.Size = UDim2.new(0, 180, 0, 33)
Club.Font = Enum.Font.SourceSans
Club.Text = "Club:"
Club.TextColor3 = Color3.fromRGB(0, 0, 0)
Club.TextScaled = true
Club.TextSize = 14.000
Club.TextWrapped = true

Casino.Name = "Casino"
Casino.Parent = Frame
Casino.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Casino.BackgroundTransparency = 1.000
Casino.Position = UDim2.new(0, 0, 0.505703449, 0)
Casino.Size = UDim2.new(0, 180, 0, 33)
Casino.Font = Enum.Font.SourceSans
Casino.Text = "Casino:"
Casino.TextColor3 = Color3.fromRGB(0, 0, 0)
Casino.TextScaled = true
Casino.TextSize = 14.000
Casino.TextWrapped = true

Bank.Name = "Bank"
Bank.Parent = Frame
Bank.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Bank.BackgroundTransparency = 1.000
Bank.Position = UDim2.new(0, 0, 0.680608392, 0)
Bank.Size = UDim2.new(0, 180, 0, 33)
Bank.Font = Enum.Font.SourceSans
Bank.Text = "Bank:"
Bank.TextColor3 = Color3.fromRGB(0, 0, 0)
Bank.TextScaled = true
Bank.TextSize = 14.000
Bank.TextWrapped = true

Pyramid.Name = "Pyramid"
Pyramid.Parent = Frame
Pyramid.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Pyramid.BackgroundTransparency = 1.000
Pyramid.Position = UDim2.new(0, 0, 0.847908735, 0)
Pyramid.Size = UDim2.new(0, 180, 0, 33)
Pyramid.Font = Enum.Font.SourceSans
Pyramid.Text = "Pyramid:"
Pyramid.TextColor3 = Color3.fromRGB(0, 0, 0)
Pyramid.TextScaled = true
Pyramid.TextSize = 14.000
Pyramid.TextWrapped = true

UICorner_2.Parent = TextButton


-- Scripts:

local function KCYZSR_fake_script() -- ScreenGui.Script 
	local script = Instance.new('Script', ScreenGui)

local sc = game.CoreGui.ScreenGui
	
	if (game:GetService("ReplicatedStorage").HeistStatus.Jewel.Locked.Value == true) then
		game.CoreGui.ScreenGui.Frame.Jewel.Text = "Jewel: Closed"
	elseif (game:GetService("ReplicatedStorage").HeistStatus.Jewel.Locked.Value == false) then
		game.CoreGui.ScreenGui.Frame.Jewel.Text = "Jewel: Open"
		end
		
	
	if (game:GetService("ReplicatedStorage").HeistStatus.Club.Locked.Value == true) then
		game.CoreGui.ScreenGui.Frame.Club.Text = "Club: Closed"
	elseif (game:GetService("ReplicatedStorage").HeistStatus.Club.Locked.Value == false) then
		game.CoreGui.ScreenGui.Frame.Club.Text = "Club: Open"
		end
		
	
	if (game:GetService("ReplicatedStorage").HeistStatus.Casino.Locked.Value ==true) then
		game.CoreGui.ScreenGui.Frame.Casino.Text = "Casino: Closed"
	elseif (game:GetService("ReplicatedStorage").HeistStatus.Casino.Locked.Value ==false) then
		game.CoreGui.ScreenGui.Frame.Casino.Text = "Casino: Open"
		end
		
	
		if (game:GetService("ReplicatedStorage").HeistStatus.Bank.Locked.Value == true) then
		game.CoreGui.ScreenGui.Frame.Bank.Text = "Bank: Closed"
	elseif (game:GetService("ReplicatedStorage").HeistStatus.Bank.Locked.Value ==false) then
		game.CoreGui.ScreenGui.Frame.Bank.Text = "Bank: Open"
		end
		if (game:GetService("ReplicatedStorage").HeistStatus.Pyramid.Locked.Value ==true) then
		game.CoreGui.ScreenGui.Frame.Pyramid.Text = "Pyramid: Closed"
	elseif (game:GetService("ReplicatedStorage").HeistStatus.Pyramid.Locked.Value == false) then
		game.CoreGui.ScreenGui.Frame.Pyramid.Text = "Pyramid: Open"
		end
	
end
coroutine.wrap(KCYZSR_fake_script)()
