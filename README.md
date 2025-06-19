<!DOCTYPE html><html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FermoLandBot WebApp</title>
  <script src="https://telegram.org/js/telegram-web-app.js"></script>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #a8e063, #56ab2f);
      color: #fff;
      text-align: center;
      padding: 40px 20px;
    }
    h1 {
      font-size: 2.2em;
      margin-bottom: 10px;
    }
    p {
      font-size: 1.2em;
    }
    .start-button {
      margin-top: 30px;
      padding: 15px 30px;
      font-size: 1em;
      background-color: #fff;
      color: #56ab2f;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      box-shadow: 0 4px 6px rgba(0,0,0,0.3);
      transition: transform 0.2s;
    }
    .start-button:hover {
      transform: scale(1.05);
    }
  </style>
</head>
<body>
  <h1>🌾 Добро пожаловать в FermoLand!</h1>
  <p>Управляй своей фермой прямо здесь.</p>
  <button class="start-button" onclick="Telegram.WebApp.close();">
    🚜 Начать играть
  </button>  <script>
    const tg = Telegram.WebApp;
    tg.expand();
  </script></body>
</html>
