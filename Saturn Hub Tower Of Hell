local ArrayField = loadstring(game:HttpGet("https://raw.githubusercontent.com/Hosvile/Refinement/main/MC%3AArrayfield%20Library"))()

local Window = ArrayField:CreateWindow({
   Name = "Saturn Hub🪐 l Tower Of Hell",
   LoadingTitle = "Saturn Hub🪐🥶",
   LoadingSubtitle = "by Retro",
   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "SaturnHub🪐"
   },
        Discord = {
            Enabled = false,
            Invite = "https://discord.com/invite/s6Mt8aXm", -- The Discord invite code, do not include discord.gg/
            RememberJoins = true -- Set this to false to make them join the discord every time they load it up
        },
        KeySystem = true, -- Set this to true to use our key system
        KeySettings = {
            Title = "Saturn Hub🪐 l Key System🔑",
            Subtitle = "Key System🔑",
            Note = "Join the discord (https://discord.com/invite/s6Mt8aXm)",
            FileName = "Saturn Keys",
            SaveKey = false,
            GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like ArrayField to get the key from
            Key = {"D38GHA6SATURN",'Hi extra'},
            Actions = {
                [1] = {
                    Text = 'Click Me To Get Saturn Key',
                    OnPress = function()
setclipboard("https://link-center.net/1015334/first-key") 
                    end,
                }
            },
        }
    })
    
local Tab1 = Window:CreateTab("AutoFarms", 5205790826)

local Tab2 = Window:CreateTab("Credits", 5205790826) -- Title, Image

local Section = Tab2:CreateSection("By Walter Christian Carlos",false) -- The 2nd argument is to tell if its only a Title and doesnt contain element

ArrayField:Notify({
   Title = "Reminder:",
   Content = "You Cant Steal Script💀",
   Duration = 6.5,
   Image = 4483362458,
   Actions = { -- Notification Buttons
      Ignore = {
         Name = "Okay?",
         Callback = function()
         print("The user tapped Okay!")
      end
   },
 },
})

local Button = Tab1:CreateButton({
   Name = "Anti Cheat",
   Interact = 'Click',
   Callback = function()
local function DisableSignal(signal, name)
    local successes = true
    for i, connection in next, getconnections(signal) do
        local success, err = pcall(connection.Disable)
        if success then
            print('successfully disconnected ' .. name .. '\'s #' .. tostring(i) .. ' connection')
        else
            if err then
                print('failed to disconnect ' .. name .. '\'s # ' .. tostring(i) .. 'connection due to ' .. err)
            end
            successes = false
        end
    end
    return successes
end

local localscript = game:GetService'Players'.LocalPlayer.PlayerScripts.LocalScript
local localscript2 = game:GetService'Players'.LocalPlayer.PlayerScripts.LocalScript2

local localscriptSignal = localscript.Changed
local localscript2Signal = localscript2.Changed

if DisableSignal(localscriptSignal, 'localscript') then
    localscript:Destroy()
end
if DisableSignal(localscript2Signal, 'localscript2') then
    localscript2:Destroy()
end
   end,
})

local Button = Tab1:CreateButton({
   Name = "Infinite Jump",
   Interact = 'Click',
   Callback = function()
		local thing = Instance.new("Part")
        thing.Name = "This is a part of the game"
        thing.Anchored = true
        thing.Parent = game.Workspace
        thing.Size = Vector3.new(5, 0.1, 5)
		thing.Transparency = 1
	game:GetService("RunService").Stepped:connect(
            function()
			local pos = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
        thing.CFrame = CFrame.new(pos.X, pos.Y-3.3,pos.Z)--beetween -3.1 and idk but prob -3.6
		end)
   end,
})

local Toggle = Tab1:CreateToggle({
   Name = "Godmode",
   CurrentValue = false,
   Flag = "Toggle1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
   local LocalPlayer = game:GetService("Players").LocalPlayer

local function Invincibility()
    if LocalPlayer.Character then
        for i, v in pairs(LocalPlayer.Character:GetChildren()) do
            if v.Name == "hitbox" then
                v:Destroy()
            end
        end
    end
end

while wait(0.5) do
    Invincibility(LocalPlayer)
end
end,
})

local Button = Tab1:CreateButton({
   Name = "Get All Items",
   Interact = 'Click',
   Callback = function()
for _,e in pairs(game.Players.LocalPlayer.Backpack:GetDescendants()) do
if e:IsA("Tool") then
e:Destroy()
end
end
wait()
for _,v in pairs(game.ReplicatedStorage.Gear:GetDescendants()) do
if v:IsA("Tool") then
local CloneThings = v:Clone()
wait()
CloneThings.Parent = game.Players.LocalPlayer.Backpack
end
end
   end,
})

local Toggle = Tab1:CreateToggle({
   Name = "Auto Farm",
   CurrentValue = false,
   Flag = "Toggle1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
   local P = game:GetService'Players'
local HRP = P.LocalPlayer.Character.HumanoidRootPart
local Sections = game:GetService("Workspace").tower.sections

for _, Child in next, Sections:GetChildren() do
if Child.Name ~= "start" then
HRP.CFrame = Child.start.CFrame + Vector3.new(1,2,1)
task.wait()
end
end
HRP.CFrame = Sections.finish.FinishGlow.CFrame
end,
})

local Toggle = Tab1:CreateToggle({
   Name = "Bot Spamer",
   CurrentValue = false,
   Flag = "Toggle1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
   local message = "Saturn Hub Op 🪐" -- the message
local Tiemlolol = 2 -- the wait time between chats, anything under 2 isnt recommended


-- Script (dont modify)

if _G.AutoSay then _G.AutoSay = false
else _G.AutoSay = true
end
while _G.AutoSay do
	local args = {[1] = message,[2] = "All"}
	game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
	task.wait(tonumber(Tiemlolol))
end
   end,
})

local Button = Tab1:CreateButton({
   Name = "Delete All KillParts",
   Interact = 'Click',
   Callback = function()
for i,v in pairs(game:GetService("Workspace").tower:GetDescendants()) do
    if v:IsA("BoolValue") and v.Name == "kills" then
        v.Parent:Destroy()
    end
end
   end,
})

local Button = Tab1:CreateButton({
   Name = "Teleport To End",
   Interact = 'Click',
   Callback = function()
   game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").tower.finishes:GetChildren()[1].CFrame
   end,
})
