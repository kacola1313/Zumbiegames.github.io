# kacola1313.github.io.-- Nightmare Hub + Zumbie Games (Guest Version)
-- By @isagilegal1313 | zumbie_games | https://kacola1313.github.io/

-- Copia automaticamente o link da página de Key
setclipboard("https://kacola1313.github.io/")
print("Link copiado! Acesse https://kacola1313.github.io/ para pegar a Ken.")

-- Janela de input para digitar a Ken
local key = tostring(game:GetService("Players").LocalPlayer:Kick("Digite a Key no chat ou script."))

-- Exemplo simples de verificação manual via chat
game:GetService("Players").LocalPlayer.Chatted:Connect(function(msg)
    if msg == "z0mb13_g4m3s141511" then
        print("Key correta! Nightmare Hub desbloqueado.")
        -- Coloque aqui o carregamento real do seu hub:
        -- loadstring(game:HttpGet("LINK_DO_HUB"))()
    else
        print("Key incorreta.")
    end
end)
