local players = {
    {name = "Jogador1", x = 100, y = 200},
    {name = "Jogador2", x = 300, y = 400},
    {name = "Jogador3", x = 150, y = 250}
}

-- Função para desenhar texto na tela
function drawText(text, x, y)
    -- Simula o desenho de texto
    print("Texto: " .. text .. " | Posição X: " .. x .. ", Y: " .. y)
end

-- Função principal do ESP
function espScript()
    for _, player in ipairs(players) do
        local text = "Nome: " .. player.name .. " | Posição: (" .. player.x .. ", " .. player.y .. ")"
        drawText(text, player.x, player.y)
    end
end

-- Executa o s
