# while wait() do

     pcall(function()

       for i,v in pairs(game.Players:GetChildren()) do

            if not v.Character.Head:FindFirstChild("ESP") and tostring(v.Team) = game. Players.LocalPpayers then

                local BillboardGui = Instance.new("BillboardGui")

                local TextLabel = Instance.new("TextLabel")

                BillboardGui.Parent = v.Character.Head

                BillboardGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

                BillboardGui.Active = true

                BillboardGui.Name = "ESP"

                BillboardGui.AlwaysOnTop = true

                BillboardGui.LightInfluence = 1.000

                BillboardGui.Size = UDim2.new(0, 60, 0, 50)

                BillboardGui.StudsOffset = Vector3.new(0, 2.5, 0)

                TextLabel.Parent = BillboardGui

                TextLabel.BackgroundColor3 = Color3.fromRGB(0, 255, 0)

                TextLabel.BackgroundTransparency = 1.000

                TextLabel.Size = UDim2.new(0, 65, 0, 50)

                TextLabel.Font = Enum.Font.GothamBold

                TextLabel.Text = v.Name

                TextLabel.TextColor3 = Color3.fromRGB(0, 255, 0)

                TextLabel.TextScaled = true

                TextLabel.TextSize = 14.000

                TextLabel.TextStrokeTransparency = 0.000

                TextLabel.TextWrapped = true

            end

        end

    end) 

end
