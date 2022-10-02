local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Sem nome.", "Sentinel")

local Tab = Window:NewTab("Inicio")
local Section = Tab:NewSection("Seja bem vindo a esse fuck hub")

local Tab = Window:NewTab("Scripts Trolls")
local Section = Tab:NewSection("Nesta pagina contém scripts e fds")
Section:NewButton("Kidnap", "Aperte Z perto do player.", function()
    game.Players.LocalPlayer:GetMouse().KeyDown:connect(function(key)
if key == 'z' then
local h = game.Players.LocalPlayer.Character.Humanoid:Clone()
local plr = game.Players.LocalPlayer.Character
local CF = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
local lp = game.Players.LocalPlayer

h.Parent = game.Players.LocalPlayer.Character
h.Name = "Hum"

game.Players.LocalPlayer.Character.Humanoid:Destroy()

for _,v in pairs(game.Players.LocalPlayer:GetDescendants()) do
    if v.ClassName == "Tool" then
        v.Parent = plr
    end
end
wait(.5)
tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(300, Enum.EasingStyle.Linear)

tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(0, -1000, 0)})
tween:Play()
end
end)
end)

local Tab = Window:NewTab("Scripts FEs")
local Section = Tab:NewSection("Nesta pagina contém scripts e fuedase")

local Tab = Window:NewTab("Hubs do playhard")
local Section = Tab:NewSection("Nesta pagina contém scripts e fuedase")
