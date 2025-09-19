<!DOCTYPE html>
<html lang="mn">
<head>
  <meta charset="UTF-8">
  <title>Бөртө минь ❤️</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      color: #fff;
      height: 100vh;
      margin: 0;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
    h1 {
      font-size: 2.5em;
      margin-bottom: 40px;
    }
    button {
      background: #ff4b5c;
      border: none;
      color: white;
      padding: 15px 30px;
      margin: 10px;
      border-radius: 30px;
      font-size: 18px;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover {
      background: #ff6f91;
      transform: scale(1.1);
    }
    .page {
      display: none;
    }
    .active {
      display: block;
      animation: fadeIn 1s;
    }
    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }
  </style>
</head>
<body>

  <!-- Эхний хуудас -->
  <div id="page1" class="page active">
    <h1>💖 Миний хайр мундаг шүү! 💖</h1>
    <button onclick="nextPage('page2')">Мэдийшдээ 😊</button>
    <button onclick="nextPage('page3')">Миний хайр жихсэн мундаг шүү 😍</button>
  </div>

  <!-- Хоёр дахь хуудас (Мэдийшдээ) -->
  <div id="page2" class="page">
    <h1>💕 Зөндөө хайртай шүү 😘💕</h1>
  </div>

  <!-- Гурав дахь хуудас (Жихсэн мундаг шүү) -->
  <div id="page3" class="page">
    <h1>🥰 Ийм хөөрхөн мундаг найз охинтой юм чинь мундаг байхгүй гээд яахав дээ ❤️</h1>
  </div>

  <script>
    function nextPage(pageId) {
      document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
      document.getElementById(pageId).classList.add('active');
    }
  </script>

</body>
</html>

