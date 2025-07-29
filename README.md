<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>I Love You Dyah 😘</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: #ffe6f0;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      text-align: center;
      color: #ff4d6d;
      overflow: hidden;
    }

    h1 {
      font-size: 3em;
      margin-top: 100px;
      animation: goyang 2s infinite;
    }

    p {
      font-size: 1.5em;
      margin: 20px;
    }

    .heart {
      font-size: 50px;
      animation: degdeg 1.2s infinite;
    }

    @keyframes degdeg {
      0% { transform: scale(1); }
      50% { transform: scale(1.3); }
      100% { transform: scale(1); }
    }

    @keyframes goyang {
      0%, 100% { transform: rotate(0deg); }
      25% { transform: rotate(1deg); }
      75% { transform: rotate(-1deg); }
    }

    .bubble {
      position: absolute;
      font-size: 24px;
      animation: floatUp 6s infinite;
      color: #ff99c8;
    }

    @keyframes floatUp {
      0% {
        bottom: -50px;
        left: calc(100% * var(--pos));
        opacity: 1;
      }
      100% {
        bottom: 100%;
        left: calc(100% * var(--pos) + 50px);
        opacity: 0;
      }
    }

    .footer {
      position: absolute;
      bottom: 20px;
      width: 100%;
      font-size: 1em;
      color: #a64d79;
    }
  </style>
</head>
<body>

  <div class="heart">💘</div>
  <h1>Hai Dyah Rizky Nur Anggraini 😚</h1>
  <p>Aku punya pengumuman penting nih...</p>
  <p><strong>AKU CINTA KAMU BANGETTT 💖💖💖</strong></p>
  <p>Saking cintanya, aku rela makan seblak level 10 demi kamu! 😱🌶️</p>
  <div class="heart">💞</div>

  <div class="footer">
    Dari pacarmu yang ngebucin 24/7 🐶❤️
  </div>

  <!-- Bubble Hati Terbang -->
  <script>
    const emojis = ['💖','💕','💘','💗','💓','💞','💝'];
    for (let i = 0; i < 20; i++) {
      const b = document.createElement('div');
      b.classList.add('bubble');
      b.innerText = emojis[Math.floor(Math.random() * emojis.length)];
      b.style.setProperty('--pos', Math.random());
      b.style.left = Math.random() * 100 + 'vw';
      b.style.animationDelay = Math.random() * 5 + 's';
      document.body.appendChild(b);
    }
  </script>

</body>
</html>
