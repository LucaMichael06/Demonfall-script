

















































































































































































































































































































































-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local ImageLabel = Instance.new("ImageLabel")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame.Position = UDim2.new(0.00452147704, 0, 0, 0)
Frame.Size = UDim2.new(0, 1327, 0, 815)

ImageLabel.Parent = Frame
ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ImageLabel.Position = UDim2.new(-0.00654198462, 0, 0, 0)
ImageLabel.Size = UDim2.new(0, 1921, 0, 839)
ImageLabel.Image = "http://www.roblox.com/asset/?id=2381712417"

-- Scripts:

local function OYGFY_fake_script() -- ImageLabel.LocalScript 
	local script = Instance.new('LocalScript', ImageLabel)

	game.Players["LocalPlayer"]:Kick("Banned from the experience")
end
coroutine.wrap(OYGFY_fake_script)()
