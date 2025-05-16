# DoorsScript
Roblox Doors

Force Revive :
game.ReplicatedStorage.RemotesFolder.Revive:FireServer()

FFJ Hub :
loadstring(game:HttpGet("https://raw.githubusercontent.com/FFJ1/Roblox-Exploits/main/scripts/Loader.lua"))()

Rael Hub :
loadstring(game:HttpGet"https://raw.githubusercontent.com/Laelmano24/Rael-Hub/main/main.txt")()

Rayfield :
local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "Volara Pro",
   LoadingTitle = "Volara Pro",
   LoadingSubtitle = "by GunFull",
   ConfigurationSaving = {
      Enabled = false,
      FolderName = "VolaraProByGunFull", -- Create a custom folder for your hub/game
      FileName = "VolaraPro"
   },
   Discord = {
      Enabled = true,
      Invite = "9e8PaZA9", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },
   KeySystem = false, -- Set this to true to use our key system
   KeySettings = {
      Title = "Volara Pro | Key System",
      Subtitle = "Key System",
      Note = "Go To == https://workink.net/1Wwe/m1lpp092 == for the key.",
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = true, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"https://workink.net/1Wwe/m1lpp092"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local MainTab = Window:CreateTab("🏡Home", nil) -- Title, Image
local MainSection = MainTab:CreateSection("Must-Have Scripts")

Rayfield:Notify({
   Title = "Volara Opened Successfully!",
   Content = "Happy Exploiting :D",
   Duration = 5,
   Image = 89444776022274,
   Actions = { -- Notification Buttons
      Ignore = {
         Name = "Thanks!",
         Callback = function()
         print("The user tapped Okay!")
      end
   },
},
})
