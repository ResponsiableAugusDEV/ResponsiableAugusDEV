local Settings = {
	JoinTeam = "Marines";
	Translator = true;
}
local Players = game:GetService("Players")
local player = Players.LocalPlayer
local screenGui = Instance.new("ScreenGui")
screenGui.Name = "AutoUI"
screenGui.Parent = player:WaitForChild("PlayerGui")
local mainFrame = Instance.new("Frame")
mainFrame.Name = "MainFrame"
mainFrame.Size = UDim2.new(0.5, 0, 0.5, 0)
mainFrame.Position = UDim2.new(0.25, 0, 0.25, 0)
mainFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
mainFrame.Parent = screenGui
local titleLabel = Instance.new("TextLabel")
titleLabel.Name = "TitleLabel"
titleLabel.Text = "Anh ĐẠT đẹp trai nhất thế giới"
titleLabel.Size = UDim2.new(1, 0, 0.2, 0)
titleLabel.BackgroundTransparency = 1
titleLabel.TextScaled = true
titleLabel.TextColor3 = Color3.new(1, 1, 1)
titleLabel.Parent = mainFrame
local closeButton = Instance.new("TextButton")
closeButton.Name = "CloseButton"
closeButton.Text = "X"
closeButton.Size = UDim2.new(0.1, 0, 0.1, 0)
closeButton.Position = UDim2.new(0.9, 0, 0, 0)
closeButton.BackgroundColor3 = Color3.fromRGB(200, 0, 0)
closeButton.TextScaled = true
closeButton.TextColor3 = Color3.new(1, 1, 1)
closeButton.Parent = mainFrame

closeButton.MouseButton1Click:Connect(function()
	screenGui:Destroy()
end)
local farmBonesButton = Instance.new("TextButton")
farmBonesButton.Name = "FarmBonesButton"
farmBonesButton.Text = "Farm Bones"
farmBonesButton.Size = UDim2.new(0.3, 0, 0.1, 0)
farmBonesButton.Position = UDim2.new(0.35, 0, 0.8, 0)
farmBonesButton.BackgroundColor3 = Color3.fromRGB(100, 100, 200)
farmBonesButton.TextScaled = true
farmBonesButton.TextColor3 = Color3.new(1, 1, 1)
farmBonesButton.Parent = mainFrame

farmBonesButton.MouseButton1Click:Connect(function()
	print("Farm Bones activated")
end)
local farmBonesButton = Instance.new("TextButton")
farmBonesButton.Name = "FarmBonesButton"
farmBonesButton.Text = "Farm Bones: OFF"
farmBonesButton.Size = UDim2.new(0.3, 0, 0.1, 0)
farmBonesButton.Position = UDim2.new(0.35, 0, 0.8, 0)
farmBonesButton.BackgroundColor3 = Color3.fromRGB(100, 100, 200)
farmBonesButton.TextScaled = true
farmBonesButton.TextColor3 = Color3.new(1, 1, 1)
farmBonesButton.Parent = mainFrame
local farmBonesActive = false

local function toggleFarmBones()
	farmBonesActive = not farmBonesActive
	if farmBonesActive then
		farmBonesButton.Text = "Farm Bones: ON"
		print("Farm Bones activated")
	else
		farmBonesButton.Text = "Farm Bones: OFF"
		print("Farm Bones deactivated")
		-- Thêm mã dừng farm bones của bạn vào đây
	end
end
farmBonesButton.MouseButton1Click:Connect(toggleFarmBones)
local moveButton = Instance.new("TextButton")
moveButton.Name = "MoveButton"
moveButton.Text = "Dịch chuyển: OFF"
moveButton.Size = UDim2.new(0.3, 0, 0.1, 0)
moveButton.Position = UDim2.new(0.35, 0, 0.65, 0)
moveButton.BackgroundColor3 = Color3.fromRGB(100, 200, 100)
moveButton.TextScaled = true
moveButton.TextColor3 = Color3.new(1, 1, 1)
moveButton.Parent = mainFrame

local moveActive = false

local function toggleMove()
	moveActive = not moveActive
	if moveActive then
		moveButton.Text = "Dịch chuyển: ON"
		print("Dịch chuyển activated")
	else
		moveButton.Text = "Dịch chuyển: OFF"
		print("Dịch chuyển deactivated")
	
	end
end

moveButton.MouseButton1Click:Connect(toggleMove)- 👋 Hi, I’m @ResponsiableAugusDEV
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
ResponsiableAugusDEV/ResponsiableAugusDEV is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
