local ScreenGui = Instance.new("ScreenGui")
local main = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local UICorner = Instance.new("UICorner")
local UICorner_2 = Instance.new("UICorner")
local TextButton = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local TextLabel_2 = Instance.new("TextLabel")
local UICorner_4 = Instance.new("UICorner")

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

main.Name = "main"
main.Parent = ScreenGui
main.BackgroundColor3 = Color3.fromRGB(85, 170, 255)
main.Position = UDim2.new(0.692727268, 0, 0.59523809, 0)
main.Size = UDim2.new(0, 185, 0, 163)
main.Active = true
main.Draggable = true

TextLabel.Parent = main
TextLabel.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
TextLabel.Position = UDim2.new(0.131663442, 0, -0.00480529666, 0)
TextLabel.Size = UDim2.new(0, 145, 0, 60)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "Welcome to Owl hub loader"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextSize = 14.000

UICorner.Parent = TextLabel

UICorner_2.Parent = main

TextButton.Parent = main
TextButton.BackgroundColor3 = Color3.fromRGB(85, 255, 0)
TextButton.Position = UDim2.new(0.0851437151, 0, 0.58788389, 0)
TextButton.Size = UDim2.new(0, 162, 0, 49)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = "Load me! Arsenal Aimbot"
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextSize = 14.000
TextButton.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/CriShoux/OwlHub/master/OwlHub.txt"))();
end)

UICorner_3.Parent = TextButton

TextLabel_2.Parent = main
TextLabel_2.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
TextLabel_2.Position = UDim2.new(0.25, 0, 0.361963183, 0)
TextLabel_2.Size = UDim2.new(0, 100, 0, 28)
TextLabel_2.Font = Enum.Font.SourceSans
TextLabel_2.Text = "Version: 1.0.0"
TextLabel_2.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.TextSize = 14.000

UICorner_4.Parent = TextLabel_2
