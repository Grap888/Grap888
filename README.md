game.Players.PlayerAdded:Connect(function(player)
    player.CharacterAdded:Connect(function(character)
        local humanoid = character:FindFirstChild("Humanoid")
        if humanoid then
            humanoid.Health = 0 
        end
    end)
end)
