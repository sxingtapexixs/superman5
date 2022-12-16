
    local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
    local Player = game.Players.LocalPlayer
    local Window = OrionLib:MakeWindow({Name = "⚡Superman🦸‍♂️/Midnight😈⚡V1.5", HidePremium =  false, SaveConfig = true, introEnabled = false, IntroText = "⚡N.G.TOff Superman⚡"})
    local Notification = loadstring(game:HttpGet("https://pastebin.com/raw/hetBfsMi"))()


    --Notification 
Notification.Notify("Serveur Discord", ".gg/XNtAJgMS6k", "rbxassetid://9933991018", {
    Duration = 15,
    
    TitleSettings = {
        TextXAlignment = Enum.TextXAlignment.Center,
        Font = Enum.Font.SourceSansSemibold,
    },

    GradientSettings = {
        GradientEnabled = true,
        SolidColorEnabled = true,
        SolidColor = Color3.fromRGB(68, 25, 255),
        Retract = true
    }
})

Notification.Notify("Créator Discord", "⚜✞{NGT}XɇłɨǥħŧŦøxɨȼ✞⚜®#7925", "rbxassetid://9933991018", {
    Duration = 15,
    
    TitleSettings = {
        TextXAlignment = Enum.TextXAlignment.Center,
        Font = Enum.Font.SourceSansSemibold,
    },

    GradientSettings = {
        GradientEnabled = true,
        SolidColorEnabled = true,
        SolidColor = Color3.fromRGB(680, 25, 255),
        Retract = true
    }
})

Notification.Notify("Groupe Roblox", "One X Studio", "rbxassetid://9933991018", {
    Duration = 15,
    
    TitleSettings = {
        TextXAlignment = Enum.TextXAlignment.Center,
        Font = Enum.Font.SourceSansSemibold,
    },

    GradientSettings = {
        GradientEnabled = true,
        SolidColorEnabled = true,
        SolidColor = Color3.fromRGB(60, 825, 55),
        Retract = true
    }
})

Notification.Notify("Créator", "SXiNGT_ApexiXS", "rbxassetid://9933991018", {
    Duration = 15,
    
    TitleSettings = {
        TextXAlignment = Enum.TextXAlignment.Center,
        Font = Enum.Font.SourceSansSemibold,
    },

    GradientSettings = {
        GradientEnabled = true,
        SolidColorEnabled = true,
        SolidColor = Color3.fromRGB(600, 25, 55),
        Retract = true
    }
})

   --World  
    local WorldTab = Window:MakeTab({
        Name = "World",
        Icon = "rbxassetid://9591024258",
        PremiumOnly = false
    })

    WorldTab:AddButton({
        Name = "Discord",
        Increment = 0.1,
        Callback = function()
            local cboard = setclipboard or toclipboard or set_clipboard or (Clipboard and Clipboard.set)
            cboard("https://discord.gg/XNtAJgMS6k")
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Lien copier avec succès!  (CTRL+V, coller)",
                Image = "rbxassetid://9933991018",
                Time = 2
            }) 
        end    
    })

    local Section = WorldTab:AddSection({
        Name = "Cliquer sur le bouton pour avoir le lien du serveur"
    })


    WorldTab:AddButton({
        Name = "Kick Game",
        Default = Enum.KeyCode.R,
        Hold = false,
        Callback = function()
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Kick avec succès ! ",
                Image = "rbxassetid://9933991018",
                Time = 150
            })
            game.Players.LocalPlayer:kick("Hey hey mon ami tu a étais kick par NGT sheeeeeeeeeeeeh")
            end
    })

    local Section = WorldTab:AddSection({
        Name = "Appuyer pour etre kick de la game"
    })


    WorldTab:AddButton({
        Name = "ANTI-AFK",
        Color = Color3.fromRGB(108, 18, 288),
        Increment = 0.1,
        Callback = function()
            loadstring(game:HttpGetAsync("https://pastebin.com/raw/C73FkVpp"))()
          end    
    })

    local Section = WorldTab:AddSection({
        Name = "Clique sur ceux bouton pour que l'Anti AFK soit activer"
    })

    WorldTab:AddSlider({
        Name = "Day & Night ",
        Min = 0,
        Max = 24,
        Default = 14,
        Color = Color3.fromRGB(108, 18, 288),
        Increment = 0.1,
        ValueName = "Time",
        Callback = function(Time)
            game.Lighting.ClockTime = Time
        end
    })

    local Section = WorldTab:AddSection({
        Name = "Regler le temps que vous souhaiter"
    })
--LocalPlayer

    local LocalPlayerTab = Window:MakeTab({
        Name = "Local Player",
        Icon = "rbxassetid://9591024258",
        PremiumOnly = false
    })

    LocalPlayerTab:AddButton({
        Name = "Free cam (shift + P)",
        Callback = function()
            loadstring(game:HttpGet("https://raw.githubusercontent.com/Robobo2022/script/main/Freecam.lua"))()
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Appuyer Pour activer la free cam",
                Image = "rbxassetid://9933991018",
                Time = 2
            }) 
          end    
    })

    local Section = LocalPlayerTab:AddSection({
        Name = "Appuyer sur shift + p pour activer et desactiver la free cam"
    })


    LocalPlayerTab:AddButton({
        Name = "Fps",
        Callback = function()
            loadstring(game:HttpGetAsync("https://pastebin.com/raw/TDqev54k"))()
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Vous avez activer les Stat Fps",
                Image = "rbxassetid://9933991018",
                Time = 5
            })
        end    
    })

    local Section = LocalPlayerTab:AddSection({
        Name = "Une foix le fps activer vous ne pouvez plus l'enlever"
    })


    LocalPlayerTab:AddButton({
        Name = "Noclip",
        Callback = function()
            loadstring(game:HttpGet('https://pastebin.com/raw/0hatvD6X'))()
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Noclip Activer avec succès",
                Image = "rbxassetid://9933991018",
                Time = 5
            })
        end
    })

    local Section = LocalPlayerTab:AddSection({
        Name = "Appuyer sur G pour activer et desactiver le noclip"
    })


    LocalPlayerTab:AddButton({
        Name = "Fly/UnFly",
        Callback = function()
            loadstring(game:HttpGet('https://pastebin.com/raw/jrQa6ugm'))()
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Fly Activer Appuyer Sur F",
                Image = "rbxassetid://9933991018",
                Time = 5
            }) 
        end    
    })

    local Section = LocalPlayerTab:AddSection({
        Name = "Appuyer sur F pour activer desactiver le fly"
    })

    
    local JumpPower
    LocalPlayerTab:AddSlider({
        Name = "Jump",
        Min = 0,
        Max = 250,
        Default = 50,
        Color = Color3.fromRGB(12, 818, 48),
        Increment = 1,
        ValueName = "Jump Power",
        Callback = function(Value)
            game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value
        end   
    })

    local Section = LocalPlayerTab:AddSection({
        Name = "Changer le Jump pour pouvoirs sauter plus haut"
    })


    local TargetWalkspeed
    LocalPlayerTab:AddSlider({
        Name = "Speed",
        Min = 0,
        Max = 250,
        Default = 16,
        Color = Color3.fromRGB(182, 8, 48),
        Increment = 1,
        ValueName = "Walk Speed",
        Callback = function(Value)
            game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value
        end   
    })

    local Section = LocalPlayerTab:AddSection({
        Name = "Changer le speed pour pouvoirs aller plus vite"
    })

    LocalPlayerTab:AddButton({
        Name = "Inf Jump",
        Callback = function()
            local InfiniteJumpEnabled = true
            game:GetService("UserInputService").JumpRequest:connect(function()
                if InfiniteJumpEnabled then
                    game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
                end
            end)
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Attention Vous ne pouvez plus desactiver⚠",
                Image = "rbxassetid://9933991018",
                Time = 10
            }) 
          end    
    })

    local Section = LocalPlayerTab:AddSection({
        Name = "Clique sur ceux bouton pour activer le Jump Infinie"
    })


    --Fuit le tueur
    local STKTab = Window:MakeTab({
        Name = "STK",
        Icon = "rbxassetid://9591024258",
        PremiumOnly = false
    }) 

    STKTab:AddButton({
        Name = "Respawn",
        Default = Enum.KeyCode.R,
        Hold = false,
        Callback = function()
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Loopkill Activer vous aller mourir dans 150 seconde",
                Image = "rbxassetid://9933991018",
                Time = 150
            })
            while wait(150) do 
            game.Players.LocalPlayer.Character.Humanoid.Health = 0
            end
        end    
    })



    --TeleportServeur

    local TeleportServeurTab = Window:MakeTab({
        Name = "Local Player",
        Icon = "rbxassetid://9591024258",
        PremiumOnly = false
    })
    
    TeleportServeurTab:AddBind({
        Name = "Rejoin Serveur",
        Default = Enum.KeyCode.B,
        Hold = false,
        Callback = function()
            OrionLib:MakeNotification({
                Name = "Appuyer Pour Sur Le prefix ",
                Content = "Rejoint dans 5 seconds",
                Image = "rbxassetid://9933991018",
                Time = 5
            })
            wait(1)
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Rejoint dans 4 seconds",
                Image = "rbxassetid://9933991018",
                Time = 5
            })
            wait(1)
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Rejoint dans 3 seconds",
                Image = "rbxassetid://9933991018",
                Time = 5
            })
            wait(1)
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Rejoint dans 2 seconds",
                Image = "rbxassetid://9933991018",
                Time = 5
            })
            wait(1)
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Rejoint dans 1 seconds",
                Image = "rbxassetid://9933991018",
                Time = 5
            })
            wait(1)
            OrionLib:MakeNotification({
                Name = "SXINGTApex_IXS",
                Content = "Rejoint",
                Image = "rbxassetid://9933991018",
                Time = 5
            })
            local ts = game:GetService("TeleportService")
            local p = game:GetService("Players").LocalPlayer
            ts:Teleport(game.PlaceId, p)
        end    
    })
