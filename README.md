# kacola1313.github.io.<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Nightmare Hub + Zumbie Games</title>
  <style>
    body {
      margin: 0;
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      color: white;
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      gap: 20px;
      text-align: center;
    }
    h1 {
      font-weight: 700;
      font-size: 2.5rem;
    }
    p.arroba {
      font-size: 1.25rem;
      font-style: italic;
      color: #70e1f5;
      margin-top: -10px;
    }
    button {
      padding: 15px 30px;
      border: none;
      border-radius: 12px;
      background: linear-gradient(45deg, #00f, #0ff);
      color: white;
      font-size: 18px;
      cursor: pointer;
      transition: transform 0.2s;
      min-width: 220px;
    }
    button:disabled {
      background: gray;
      cursor: not-allowed;
    }
    .links {
      display: flex;
      flex-direction: column;
      gap: 12px;
      margin-top: 10px;
      width: 250px;
    }
    .links a {
      background: linear-gradient(45deg, #6a11cb, #2575fc);
      padding: 12px;
      border-radius: 10px;
      color: white;
      font-weight: 600;
      text-decoration: none;
      font-size: 16px;
      display: block;
      transition: background 0.3s;
    }
    .links a:hover {
      background: linear-gradient(45deg, #2575fc, #6a11cb);
    }
  </style>
</head>
<body>

  <h1>Nightmare Hub + Zumbie Games</h1>
  <p class="arroba">@isagilegal1313</p>

  <button id="keyButton" disabled>1:00</button>

  <div class="links">
    <a href="https://www.tiktok.com/@zumbie_games" target="_blank" rel="noopener noreferrer">
      Assista meus vídeos no TikTok
    </a>
    <a href="https://www.tiktok.com/@zumbie_games" target="_blank" rel="noopener noreferrer">
      Me siga no TikTok
    </a>
    <a href="https://www.tiktok.com/message/@zumbie_games" target="_blank" rel="noopener noreferrer">
      Converse comigo sobre ideias (privado)
    </a>
  </div>

  <script>
    const keyButton = document.getElementById("keyButton");
    let timeLeft = 60;

    const countdown = setInterval(() => {
      timeLeft--;
      const minutes = Math.floor(timeLeft / 60);
      const seconds = timeLeft % 60;
      keyButton.innerText = `${minutes}:${seconds.toString().padStart(2, '0')}`;

      if (timeLeft <= 0) {
        clearInterval(countdown);
        keyButton.disabled = false;
        keyButton.innerText = "Copiar Ken (48h)";
        keyButton.onclick = function() {
          navigator.clipboard.writeText('z0mb13_g4m3s141511');
          alert("Ken copiada! Você tem 48 horas para usar.");
        };
      }
    }, 1000);
  </script>

</body>
</html>
