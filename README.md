                -- Create entity
                local entity3 = Creator.createEntity({
                    CustomName = "Ripper", -- Custom name of your entity
                    Model = "12262768551", -- Can be GitHub file or rbxassetid
                    Speed = 183, -- Percentage, 100 = default Rush speed
                    DelayTime = 6.7, -- Time before starting cycles (seconds)
                    HeightOffset = 9,
                    CanKill = true,
                    KillRange = 185,
                    BreakLights = false,
                    BackwardsMovement = false,
                    FlickerLights = {
                        true, -- Enabled/Disabled
                        1, -- Time (seconds)
                    },
                    Cycles = {
                        Min = 1,
                        Max = 1,
                        WaitTime = 0,
                    },
                    CamShake = {
                        true, -- Enabled/Disabled
                        {3.5, 20, 0.1, 1}, -- Shake values (don't change if you don't know)
                        100, -- Shake start distance (from Entity to you)
                    },
                    Jumpscare = {
                        false, -- Enabled/Disabled
                        {
                            Image1 = "rbxassetid://11826279255", -- Image1 url
                            Image2 = "rbxassetid://8158384019", -- Image2 url
                            Shake = true,
                            Sound1 = {
                                4067643809, -- SoundId
                                { Volume = 10 }, -- Sound properties
                            },
                            Sound2 = {
                                4067643809, -- SoundId
                                { Volume = 10 }, -- Sound properties
                            },
                            Flashing = {
                                true, -- Enabled/Disabled
                                Color3.fromRGB(255, 255, 255), -- Color
                            },
                            Tease = {
                                true, -- Enabled/Disabled
                                Min = 1,
                                Max = 1,
                            },
                        },
                    },
                    CustomDialog = {"You died to who you call Ripper...", "Try your best to out-run him.", "I really don't have nothing else", "Just try your best to Hide when you can."}, -- Custom death message
                })

                ------------------------
                Creator.runEntity(entity3)
                -- Run the created entity
            end)
        end
    end
