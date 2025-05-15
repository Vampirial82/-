<!DOCTYPE html><html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Профиль игрока - Казино Бот</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #191c29, #1f2235);
      color: white;
    }.profile {
  max-width: 800px;
  margin: auto;
  padding: 20px;
}

.card {
  background-color: #2e2f45;
  border-radius: 16px;
  padding: 20px;
  margin-bottom: 20px;
  box-shadow: 0 0 10px #00000040;
}

.card h2 {
  margin-top: 0;
  color: #ffd700;
}

.resources div {
  padding: 10px;
  margin-bottom: 8px;
  border-radius: 10px;
  background-color: #3b3d5c;
}

.badges span {
  display: inline-block;
  padding: 8px 12px;
  margin: 5px;
  background: #444a6b;
  border-radius: 10px;
  font-size: 14px;
}

ul.tasks {
  list-style: none;
  padding: 0;
}

ul.tasks li {
  background-color: #3a3c5e;
  padding: 10px;
  border-radius: 8px;
  margin-bottom: 6px;
}

  </style>
</head>
<body>
  <div class="profile">
    <div class="card">
      <h1>Профиль: <span id="username">@username</span></h1>
    </div><div class="card resources">
  <h2>Ресурсы</h2>
  <div>🪙 Монеты: <span id="coins">0</span></div>
  <div>💎 Гемы: <span id="gems">0</span></div>
  <div>☣️ Токсины: <span id="toxins">0</span></div>
  <div>🧩 Пазлы: <span id="puzzles">0</span></div>
</div>

<div class="card">
  <h2>Достижения</h2>
  <div class="badges">
    <span>🏆 Питомцевод</span>
    <span>💰 Богатый человек</span>
    <span>🏡 Домовладелец</span>
  </div>
</div>

<div class="card">
  <h2>Ежедневные задания</h2>
  <ul class="tasks">
    <li>✔️ 3x /work — <b>3/3</b></li>
    <li>⌛ 10x /spin — <b>7/10</b></li>
    <li>✔️ 3x /dice — <b>3/3</b></li>
    <li>⌛ 2x /work2 — <b>1/2</b></li>
  </ul>
</div>

  </div>  <script>
    // Здесь можно подгрузить JSON с сервера или из Telegram WebApp
    const profile = {
      username: "player123",
      coins: 15000,
      gems: 24,
      toxins: 1200,
      puzzles: 32
    };

    document.getElementById("username").textContent = `@${profile.username}`;
    document.getElementById("coins").textContent = profile.coins;
    document.getElementById("gems").textContent = profile.gems;
    document.getElementById("toxins").textContent = profile.toxins;
    document.getElementById("puzzles").textContent = profile.puzzles;
  </script></body>
</html>
