local Players = game:GetService("Players")
local HighlightService = game:GetService("Highlight")

for _, player in ipairs(Players:GetPlayers()) do
    local character = player.Character
    if character then
        local highlight = Instance.new("Highlight")
        highlight.Parent = character
        highlight.FillColor = Color3.new(1, 0, 0) -- Red color
        highlight.OutlineColor = Color3.new(1, 1, 1) -- White outline
        highlight.FillTransparency = 0.5 -- Semi-transparent
        highlight.OutlineTransparency = 0 -- Opaque outline
    end
end
