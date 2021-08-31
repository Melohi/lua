local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()
local w = library:CreateWindow("Melohub - PSX")
local b = w:CreateFolder("Diamond Dupe")
local g = w:CreateFolder("Mix")
local p = w:CreateFolder("Value Editor")
local o = w:CreateFolder("Trading")
local x = w:CreateFolder("Pet Editor")
local l = w:CreateFolder("Pet Icons")
local k = w:CreateFolder("Golden Pet Icons")
local t = w:CreateFolder("Credits")

b:Button("Coming Soon",function()
Print("Coming Soon")
end)

g:Button("Gamepasses",function()
local main = debug.getupvalues(require(game.ReplicatedStorage:WaitForChild("Framework"):WaitForChild("Library")).Save.Get)[2][game.Players.LocalPlayer].save.Gamepasses
table.insert(main,18674296)
table.insert(main,18674298)
table.insert(main,18674321)
end)

g:Button("Egg Animation Skip",function()
for i,v in pairs(getgc(true)) do
   if (typeof(v) == 'table' and rawget(v, 'OpenEgg')) then
       v.OpenEgg = function()
           return
       end
   end
end
end)

p:Box("Diamond","Value",function(value)
    game:GetService("Players").LocalPlayer.PlayerGui.Main.Right.Diamonds.Amount.Text = value
end)

p:Box("Fantasy Coins","Value",function(value)
game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Right["Fantasy Coins"].Amount.Text = value
end)

p:Box("Coins","Value",function(value)
    game:GetService("Players").LocalPlayer.PlayerGui.Main.Right.Coins.Amount.Text = value
end)

o:Box("Client's Diamonds","Value",function(value)
game:GetService("Players")["LocalPlayer"].PlayerGui.Trading.Frame.Trade.Client.Diamonds.Input.Text = value
end)

o:Box("Player's Diamonds(Patched)","Value",function(value)
game:GetService("Players")["LocalPlayer"].PlayerGui.Trading.Frame.Trade.Player.Diamonds.Amount.Text = value
end)

t:Button("Nyxspite#6666",function()
setclipboard("Nyxspite#6666")
end)

t:Button("Pojken#0001",function()
setclipboard("Pojken#0001")
end)

t:Button("Fxnd.exe#0001",function()
setclipboard("Fxnd.exe#0001")
end)

t:Button("Goldy#1337",function()
setclipboard("Goldy#1337")
end)


x:Button("Dupe Pets",function()
local shit = string.gsub(game:GetService("Players").LocalPlayer.PlayerGui.Inventory.Frame.PetAmount.Text, " Pets", "")
local bitch = string.gsub(shit, " 1", "")
local number = tonumber(bitch) + 1
game:GetService("Players").LocalPlayer.PlayerGui.Inventory.Frame.PetAmount.Text = tostring(number .. " Pets")
local copy = game:GetService("Players")["LocalPlayer"].PlayerGui.Inventory.Frame.Main.Pets.id1f7cf80bceb34ca49d0e7e99078cee53:Clone()
    copy.Parent = game:GetService("Players")["LocalPlayer"].PlayerGui.Inventory.Frame.Main.Pets

game:GetService("Players").LocalPlayer.PlayerGui.Inventory.Frame.PetAmount.Text = tostring(numbervalue .. " Pets")
end)



x:Box("Pets","Value",function(value)
 game:GetService("Players")["LocalPlayer"].PlayerGui.Inventory.Frame.PetAmount.Text = value.. " Pets"
end)

x:Box("PetIcon","Value",function(value)
game:GetService("Players")["LocalPlayer"].PlayerGui.Inventory.Frame.Main.Pets.id1f7cf80bceb34ca49d0e7e99078cee53.PetIcon.Image = value
end)

x:Box("Pet Levels(k)","Value",function(value)
game:GetService("Players")["LocalPlayer"].PlayerGui.Inventory.Frame.Main.Pets.id1f7cf80bceb34ca49d0e7e99078cee53.Level.Text = value.. "k"
end)

x:Box("Pet Levels(m)","Value",function(value)
game:GetService("Players")["LocalPlayer"].PlayerGui.Inventory.Frame.Main.Pets.id1f7cf80bceb34ca49d0e7e99078cee53.Level.Text = value.. "m"
end)

x:Button("Remove Duped Pets",function()
function getNil(name,class) for _,v in pairs(getnilinstances())do if v.ClassName==class and v.Name==name then return v;end end end

local args = {
    [1] = {
        [1] = "id1f7cf80bceb34ca49d0e7e99078cee53",
    },
}

workspace["__THINGS"]["__REMOTES"]["equip pet"]:InvokeServer(unpack(args))
wait()
function getNil(name,class) for _,v in pairs(getnilinstances())do if v.ClassName==class and v.Name==name then return v;end end end

local args = {
    [1] = {
        [1] = "id1f7cf80bceb34ca49d0e7e99078cee53",
    },
}

workspace["__THINGS"]["__REMOTES"]["unequip pet"]:InvokeServer(unpack(args))
end)

l:Dropdown("Mythicals",{"Phantom Wolf","Wyvern of Hades"},true,function(value)
    if value == "Phantom Wolf" then
    setclipboard("rbxassetid://7241297390")
    end
    if value == "Wyvern of Hades" then
    setclipboard("rbxassetid://7325315549")
    end
end)

l:Dropdown("Legendaries",{"Agony","Hound of Hades","Domortuus"},true,function(value)
    if value == "Agony" then
    setclipboard("rbxassetid://6551199736")
    end
    if value == "Hound of Hades" then
    setclipboard("rbxassetid://7102599588")
    end
    if value == "Domortuus" then
    setclipboard("rbxassetid://7035121134")
    end
end)

l:Dropdown("Epics",{"Dominus Empyreus","Dominus Infernus","Dominus Fridgidus"},true,function(value)
    if value == "Dominus Infernus" then
    setclipboard("rbxassetid://6541409389")
    end
    if value == "Dominus Fridgidus" then
    setclipboard("rbxassetid://6541409482")
    end
    if value == "Dominus Empyreus" then
    setclipboard("rbxassetid://6541409553")
    end
end)

k:Dropdown("Mythicals",{"Phantom Wolf","Wyvern of Hades"},true,function(value)
    if value == "Phantom Wolf" then
    setclipboard("rbxassetid://7241297514")
    end
    if value == "Wyvern of Hades" then
    setclipboard("rbxassetid://7325315622")
    end
end)

k:Dropdown("Legendaries",{"Agony","Hound of Hades","Domortuus"},true,function(value)
    if value == "Agony" then
    setclipboard("rbxassetid://6551199736")
    end
    if value == "Hound of Hades" then
    setclipboard("rbxassetid://7102599588")
    end
    if value == "Domortuus" then
    setclipboard("rbxassetid://7035121200")
    end
end)

k:Dropdown("Epics",{"Dominus Empyreus","Dominus Infernus","Dominus Fridgidus"},true,function(value)
    if value == "Dominus Infernus" then
    setclipboard("rbxassetid://6844994886")
    end
    if value == "Dominus Fridgidus" then
    setclipboard("rbxassetid://6844994886")
    end
    if value == "Dominus Empyreus" then
    setclipboard("rbxassetid://6844994886")
    end
end)

k:Button("Copy Pet ID",function()
local petsHolder = game:GetService("Players").LocalPlayer.PlayerGui.Inventory.Frame.Main.Pets
local petIDs = {}
for index,value in pairs(petsHolder:GetChildren()) do
if value.ClassName == "TextButton" then
table.insert(petIDs, 1, value.Name)--Print if it works cause idk how to use table.insert
for keyN, keyV in pairs(petIDs) do
setclipboard(keyV)
break
end
end
end
end)

l:Button("Copy Pet ID",function()
local petsHolder = game:GetService("Players").LocalPlayer.PlayerGui.Inventory.Frame.Main.Pets
local petIDs = {}
for index,value in pairs(petsHolder:GetChildren()) do
if value.ClassName == "TextButton" then
table.insert(petIDs, 1, value.Name)--Print if it works cause idk how to use table.insert
for keyN, keyV in pairs(petIDs) do
setclipboard(keyV)
break
end
end
end
end)
t:DestroyGui()
