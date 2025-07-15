# kacola1313.github.io<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
    }
    button {
      padding: 15px 25px;
      border: none;
      border-radius: 12px;
      background: linear-gradient(45deg, #00f, #0ff);
      color: white;
      font-size: 18px;
      cursor: pointer;
      transition: transform 0.2s;
    }
    button:disabled {
      background: gray;
      cursor: not-allowed;
    }
  </style>
</head>
<body>

  <h1>Nightmare Hub + Zumbie Games</h1>

  <button id="keyButton" disabled>Esperando 1 minuto...</button>

  <script>
    const keyButton = document.getElementById("keyButton");

    setTimeout(() => {
      keyButton.disabled = false;
      keyButton.innerText = "Copiar Ken (48h)";
      keyButton.onclick = function() {
        navigator.clipboard.writeText('z0mb13_g4m3s141511');
        alert("Ken copiada! Você tem 48 horas para usar.");
      };
    }, 60000); // 60000 milissegundos = 1 minuto
  </script>

</body>
</html>
