local ScreenGui = Instance.new("ScreenGui")
local OpenFrame = Instance.new("Frame")
local Open = Instance.new("TextButton")
local UICorner = Instance.new("UICorner")
local Main = Instance.new("Frame")
local UICorner_2 = Instance.new("UICorner")
local Label = Instance.new("TextLabel")
local Fly = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local ClicktoTp = Instance.new("TextButton")
local UICorner_4 = Instance.new("UICorner")
local InvisibleFling = Instance.new("TextButton")
local UICorner_5 = Instance.new("UICorner")
local CmdX = Instance.new("TextButton")
local UICorner_6 = Instance.new("UICorner")
local SwiftyTheDonkey = Instance.new("TextButton")
local UICorner_7 = Instance.new("UICorner")
local DarkDexExplorer = Instance.new("TextButton")
local UICorner_8 = Instance.new("UICorner")
local Close = Instance.new("TextButton")
local UICorner_9 = Instance.new("UICorner")
 
 
ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
 
OpenFrame.Name = "OpenFrame"
OpenFrame.Parent = ScreenGui
OpenFrame.BackgroundColor3 = Color3.fromRGB(74, 74, 74)
OpenFrame.Position = UDim2.new(0.00676691718, 0, 0.930197239, 0)
OpenFrame.Size = UDim2.new(0, 156, 0, 38)
 
Open.Name = "Open"
Open.Parent = OpenFrame
Open.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
Open.Position = UDim2.new(0.025641026, 0, 0.0789473653, 0)
Open.Size = UDim2.new(0, 147, 0, 31)
Open.Font = Enum.Font.SciFi
Open.Text = "DevoloperPanelOpener"
Open.TextColor3 = Color3.fromRGB(255, 255, 255)
Open.TextScaled = true
Open.TextSize = 14.000
Open.TextWrapped = true
Open.MouseButton1Click:Connect(function()
	Main.Visible = true
end)
 
UICorner.Parent = OpenFrame
 
Main.Name = "Main"
Main.Parent = ScreenGui
Main.BackgroundColor3 = Color3.fromRGB(74, 74, 74)
Main.Position = UDim2.new(0.333082736, 0, 0.257966608, 0)
Main.Size = UDim2.new(0, 230, 0, 334)
Main.Visible = false
 
UICorner_2.CornerRadius = UDim.new(0, 12)
UICorner_2.Parent = Main
 
Label.Name = "Label"
Label.Parent = Main
Label.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Label.BackgroundTransparency = 1.000
Label.Position = UDim2.new(0.0260869563, 0, -0.032934133, 0)
Label.Size = UDim2.new(0, 190, 0, 54)
Label.Font = Enum.Font.SciFi
Label.Text = "Devoloper Panel"
Label.TextColor3 = Color3.fromRGB(255, 255, 255)
Label.TextScaled = true
Label.TextSize = 14.000
Label.TextWrapped = true
 
Fly.Name = "Fly"
Fly.Parent = Main
Fly.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
Fly.Position = UDim2.new(0.14782609, 0, 0.161676645, 0)
Fly.Size = UDim2.new(0, 162, 0, 32)
Fly.Font = Enum.Font.SciFi
Fly.Text = "Fly"
Fly.TextColor3 = Color3.fromRGB(255, 255, 255)
Fly.TextScaled = true
Fly.TextSize = 14.000
Fly.TextWrapped = true
Fly.MouseButton1Click:Connect(function()
	loadstring(game:HttpGet("https://pastebin.com/raw/7rXZ9VNc", true))()
end)
 
UICorner_3.Parent = Fly
 
ClicktoTp.Name = "ClicktoTp"
ClicktoTp.Parent = Main
ClicktoTp.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
ClicktoTp.Position = UDim2.new(0.14782609, 0, 0.293413162, 0)
ClicktoTp.Size = UDim2.new(0, 162, 0, 32)
ClicktoTp.Font = Enum.Font.SciFi
ClicktoTp.Text = "Ctrl Click to TP"
ClicktoTp.TextColor3 = Color3.fromRGB(255, 255, 255)
ClicktoTp.TextScaled = true
ClicktoTp.TextSize = 14.000
ClicktoTp.TextWrapped = true
ClicktoTp.MouseButton1Click:Connect(function()
 
	local Plr = game:GetService("Players").LocalPlayer
	local Mouse = Plr:GetMouse()
 
	Mouse.Button1Down:connect(
		function()
			if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then
				return
			end
			if not Mouse.Target then
				return
			end
			Plr.Character:MoveTo(Mouse.Hit.p)
		end
	)
end)
 
 
UICorner_4.Parent = ClicktoTp
 
InvisibleFling.Name = "InvisibleFling"
InvisibleFling.Parent = Main
InvisibleFling.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
InvisibleFling.Position = UDim2.new(0.14782609, 0, 0.42814368, 0)
InvisibleFling.Size = UDim2.new(0, 162, 0, 32)
InvisibleFling.Font = Enum.Font.SciFi
InvisibleFling.Text = "InvisibleFling"
InvisibleFling.TextColor3 = Color3.fromRGB(255, 255, 255)
InvisibleFling.TextScaled = true
InvisibleFling.TextSize = 14.000
InvisibleFling.TextWrapped = true
InvisibleFling.MouseButton1Click:Connect(function()
 
 
	spawn(function()
		local message = Instance.new("Message",workspace)
		message.Text = "Loaded press z to execute inviseble , press x to respawn)"
		wait(0.5)
		message:Destroy()
	end)
 
 
 
 
 
 
 
 
	local mouse = game.Players.LocalPlayer:GetMouse()
 
	local groot = nil
 
	mouse.KeyDown:connect(function(k)
 
		if k == "z" then
 
 
 
			spawn(function()
				local message = Instance.new("Message",workspace)
				message.Text = "Fe Invisible Fling By Diemiers#4209 Loaded (wait 11 seconds to load)"
				wait(11)
				message:Destroy()
			end)
 
 
			local ch = game.Players.LocalPlayer.Character
			local prt=Instance.new("Model", workspace)
			local z1 =  Instance.new("Part", prt)
			z1.Name="Torso"
			z1.CanCollide = false
			z1.Anchored = true
			local z2  =Instance.new("Part", prt)
			z2.Name="Head"
			z2.Anchored = true
			z2.CanCollide = false
			local z3 =Instance.new("Humanoid", prt)
			z3.Name="Humanoid"
			z1.Position = Vector3.new(0,9999,0)
			z2.Position = Vector3.new(0,9991,0)
			game.Players.LocalPlayer.Character=prt
			wait(5)
			game.Players.LocalPlayer.Character=ch
			wait(6)
 
 
			local plr = game.Players.LocalPlayer
			mouse = plr:GetMouse()
 
			local Hum = Instance.new("Humanoid")
			Hum.Parent = game.Players.LocalPlayer.Character
 
 
			local root =  game.Players.LocalPlayer.Character.HumanoidRootPart
 
 
			for i,v in pairs(plr.Character:GetChildren()) do
 
				if v ~= root and  v.Name ~= "Humanoid" then
 
					v:Destroy()
 
				end
 
 
			end
 
			workspace.CurrentCamera.CameraSubject = root
 
			local se = Instance.new("SelectionBox",root)
			se.Adornee = root
 
 
			game:GetService('RunService').Stepped:connect(function()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CanCollide = false
			end)
			game:GetService('RunService').RenderStepped:connect(function()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CanCollide = false
			end)
 
 
			power = 999999 -- change this to make it more or less powerful
 
			power = power*10
 
			---
			wait(.1)
			local bambam = Instance.new("BodyThrust")
			bambam.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
			bambam.Force = Vector3.new(power,0,power)
			bambam.Location = game.Players.LocalPlayer.Character.HumanoidRootPart.Position 
 
 
 
 
 
			local plr = game.Players.LocalPlayer
			local torso = root
			local flying = true
			local deb = true
			local ctrl = {f = 0, b = 0, l = 0, r = 0}
			local lastctrl = {f = 0, b = 0, l = 0, r = 0}
			local maxspeed = 120
			local speed = 15
 
 
			---local bambam = Instance.new("BodyThrust")
			---bambam.Parent = torso
			--bambam.Force = Vector3.new(9999999,0,9999999)
			--bambam.Location = torso.Position
 
 
			---
			groot = root
 
			function Fly()
				local bg = Instance.new("BodyGyro", torso)
				bg.P = 9e4
				bg.maxTorque = Vector3.new(0, 0, 0)
				bg.cframe = torso.CFrame
				local bv = Instance.new("BodyVelocity", torso)
				bv.velocity = Vector3.new(0,0,0)
				bv.maxForce = Vector3.new(9e9, 9e9, 9e9)
				repeat wait()
 
					if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then
						speed = speed+.2
						if speed > maxspeed then
							speed = maxspeed
						end
					elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then
						speed = speed-1
						if speed < 0 then
							speed = 0
						end
					end
					if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then
						bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
						lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r}
					elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then
						bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
					else
						bv.velocity = Vector3.new(0,0.1,0)
					end
 
				until not flying
				ctrl = {f = 0, b = 0, l = 0, r = 0}
				lastctrl = {f = 0, b = 0, l = 0, r = 0}
				speed = 0
				bg:Destroy()
				bv:Destroy()
 
			end
			mouse.KeyDown:connect(function(key)
				if key:lower() == "e" then
					if flying then flying = false
					else
						flying = true
						Fly()
					end
				elseif key:lower() == "w" then
					ctrl.f = 1
				elseif key:lower() == "s" then
					ctrl.b = -1
				elseif key:lower() == "a" then
					ctrl.l = -1
				elseif key:lower() == "d" then
					ctrl.r = 1
				end
			end)
			mouse.KeyUp:connect(function(key)
				if key:lower() == "w" then
					ctrl.f = 0
				elseif key:lower() == "s" then
					ctrl.b = 0
				elseif key:lower() == "a" then
					ctrl.l = 0
				elseif key:lower() == "d" then
					ctrl.r = 0
				elseif key:lower() == "r" then
 
				end
			end)
			Fly()
 
 
 
		elseif k == "x" then
 
 
			spawn(function()
				local message = Instance.new("Message",workspace)
				message.Text = "Respawning dont spam"
				wait(1)
				message:Destroy()
			end)
 
			local saved = groot.Position
 
			local ch = game.Players.LocalPlayer.Character
			local prt=Instance.new("Model", workspace)
			local z1 =  Instance.new("Part", prt)
			z1.Name="Torso"
			z1.CanCollide = false
			z1.Anchored = true
			local z2  =Instance.new("Part", prt)
			z2.Name="Head"
			z2.Anchored = true
			z2.CanCollide = false
			local z3 =Instance.new("Humanoid", prt)
			z3.Name="Humanoid"
			z1.Position = Vector3.new(0,9999,0)
			z2.Position = Vector3.new(0,9991,0)
			game.Players.LocalPlayer.Character=prt
			wait(5)
			game.Players.LocalPlayer.Character=ch
			local poop = nil
			repeat wait() poop = game.Players.LocalPlayer.Character:FindFirstChild("Head") until poop ~= nil
			wait(1)
			game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(saved)
 
		end
 
 
	end)
end)
 
UICorner_5.Parent = InvisibleFling
 
CmdX.Name = "CmdX"
CmdX.Parent = Main
CmdX.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
CmdX.Position = UDim2.new(0.14782609, 0, 0.559880197, 0)
CmdX.Size = UDim2.new(0, 162, 0, 32)
CmdX.Font = Enum.Font.SciFi
CmdX.Text = "CmdX"
CmdX.TextColor3 = Color3.fromRGB(255, 255, 255)
CmdX.TextScaled = true
CmdX.TextSize = 14.000
CmdX.TextWrapped = true
CmdX.MouseButton1Click:Connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/CMD-X/CMD-X/master/Source", true))()
end)
 
UICorner_6.Parent = CmdX
 
SwiftyTheDonkey.Name = "SwiftyTheDonkey"
SwiftyTheDonkey.Parent = Main
SwiftyTheDonkey.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
SwiftyTheDonkey.Position = UDim2.new(0.14782609, 0, 0.688622713, 0)
SwiftyTheDonkey.Size = UDim2.new(0, 162, 0, 32)
SwiftyTheDonkey.Font = Enum.Font.SciFi
SwiftyTheDonkey.Text = "SwiftyTheDonkey"
SwiftyTheDonkey.TextColor3 = Color3.fromRGB(255, 255, 255)
SwiftyTheDonkey.TextScaled = true
SwiftyTheDonkey.TextSize = 14.000
SwiftyTheDonkey.TextWrapped = true
SwiftyTheDonkey.MouseButton1Click:Connect(function()
	loadstring(game:HttpGet("https://pastebin.com/raw/SqUvm1qF", true))()
end)
 
UICorner_7.Parent = SwiftyTheDonkey
 
DarkDexExplorer.Name = "DarkDexExplorer"
DarkDexExplorer.Parent = Main
DarkDexExplorer.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
DarkDexExplorer.Position = UDim2.new(0.14782609, 0, 0.826347291, 0)
DarkDexExplorer.Size = UDim2.new(0, 162, 0, 32)
DarkDexExplorer.Font = Enum.Font.SciFi
DarkDexExplorer.Text = "DarkDexExplorer"
DarkDexExplorer.TextColor3 = Color3.fromRGB(255, 255, 255)
DarkDexExplorer.TextScaled = true
DarkDexExplorer.TextSize = 14.000
DarkDexExplorer.TextWrapped = true
DarkDexExplorer.MouseButton1Click:Connect(function()
	loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/Shadow-Developer/Shadow/master/Scripts/DarkDexExplorer.lua"))()
end)
 
UICorner_8.Parent = DarkDexExplorer
 
Close.Name = "Close"
Close.Parent = Main
Close.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
Close.Position = UDim2.new(0.852173924, 0, 0.00598802604, 0)
Close.Size = UDim2.new(0, 32, 0, 27)
Close.Font = Enum.Font.SciFi
Close.Text = "X"
Close.TextColor3 = Color3.fromRGB(255, 10, 10)
Close.TextScaled = true
Close.TextSize = 14.000
Close.TextWrapped = true
Close.MouseButton1Click:Connect(function()
		Main.Visible = false
	end)	
 
UICorner_9.Parent = Close
