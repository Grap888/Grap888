local function killAllPlayers()
    for _, player in pairs(game.Players:GetPlayers()) do
        local character = player.Character
        if character and character:FindFirstChild("Humanoid") then
            character.Humanoid.Health = 0
        end
    end
end


local button = script.Parent  
button.MouseButton1Click:Connect(killAllPlayers)
