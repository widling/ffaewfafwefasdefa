-- Polar Ice Cap Sim Item Spawner

-- Function to spawn an item by name
local function spawnItem(itemName)
    local replicatedStorage = game:GetService("ReplicatedStorage")
    local item = replicatedStorage:FindFirstChild(itemName)

    if item then
        local clone = item:Clone()
        clone.Parent = workspace
        clone.Position = game.Players.LocalPlayer.Character.HumanoidRootPart.Position + Vector3.new(0, 5, 0)
    else
        warn("Item '" .. itemName .. "' not found in ReplicatedStorage.")
    end
end

-- List of item names to spawn
local itemsToSpawn = {
    "Drico",
    -- Add more item names as needed
}

-- Spawn the items
for _, itemName in ipairs(itemsToSpawn) do
    spawnItem(itemName)
end
