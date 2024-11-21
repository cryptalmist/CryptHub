buff script:
```lua
local player = game.Players.LocalPlayer

-- Function to set or edit custom attributes for the AccessoryEffects folder
local function editAccessoryAttributes()
    -- Reference to the AccessoryEffects folder
    local accessoryFolder = player:FindFirstChild("AccessoryEffects")
    
    if accessoryFolder then
        -- Setting or updating attributes
        accessoryFolder:SetAttribute("Lifesteal", 1)
        accessoryFolder:SetAttribute("Lightning_Chance", 0)
        accessoryFolder:SetAttribute("Melee_Range", 23)
        accessoryFolder:SetAttribute("Pogo_Range", 2)


        print("Attributes updated for AccessoryEffects folder.")
    else
        print("AccessoryEffects folder not found.")
    end
end

-- Run the function to edit attributes
editAccessoryAttributes()
```