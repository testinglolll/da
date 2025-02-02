-- Supondo que você tenha uma variável chamada "clickCooldown" controlando o tempo de espera
local clickCooldown = 0 -- Define o cooldown como 0 para remover o delay

-- Exemplo de função para usar ao clicar
local function onClick()
    -- Seu código de clique aqui, como a aplicação de força ou ação
    print("Força aplicada!")
end

-- Conecte ao evento de clique
game.Players.LocalPlayer.Mouse.Button1Down:Connect(function()
    if clickCooldown == 0 then
        onClick()
        -- Após o clique, você pode ajustar outras lógicas, como atualizar uma UI ou aplicar efeitos
    end
end)
