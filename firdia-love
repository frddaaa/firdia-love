<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Untuk Firdia 💖</title>

  <!-- QR Library -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>

  <style>
    body {
      margin: 0;
      height: 100vh;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      font-family: 'Segoe UI', sans-serif;
    }

    .card {
      background: white;
      padding: 30px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 40px rgba(0,0,0,0.2);
      z-index: 2;
      animation: fadeIn 1.2s ease;
    }

    h1 {
      color: #ff4b7d;
      margin-bottom: 10px;
    }

    p {
      color: #666;
      margin-bottom: 20px;
    }

    #qrcode {
      margin-top: 10px;
    }

    button {
      margin-top: 15px;
      padding: 10px 20px;
      border: none;
      border-radius: 10px;
      background: #ff4b7d;
      color: white;
      cursor: pointer;
    }

    /* Animasi hati */
    .heart {
      position: absolute;
      color: rgba(255,255,255,0.8);
      font-size: 20px;
      animation: fall linear infinite;
    }

    @keyframes fall {
      0% { transform: translateY(-10vh); opacity: 1; }
      100% { transform: translateY(110vh); opacity: 0; }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.8); }
      to { opacity: 1; transform: scale(1); }
    }
  </style>
</head>

<body>

  <div class="card">
    <h1>💖 Untuk Firdia 💖</h1>
    <p>Scan ini ya... ada sesuatu buat kamu 😳</p>
    <div id="qrcode"></div>

    <button onclick="playMusic()">🎵 Play Music</button>
  </div>

  <!-- Musik romantis -->
  <audio id="music" loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
  </audio>

  <script>
    // QR Code
    new QRCode(document.getElementById("qrcode"), {
      text: "aku Sayang kamu, Firdia ❤️",
      width: 200,
      height: 200,
      colorDark: "#ff4b7d",
      colorLight: "#ffffff",
      correctLevel: QRCode.CorrectLevel.H
    });

    // Autoplay (butuh interaksi dulu di beberapa HP)
    function playMusic() {
      document.getElementById("music").play();
    }

    // Auto coba play (kadang berhasil di desktop)
    window.onload = () => {
      document.getElementById("music").play().catch(() => {});
    };

    // Hati jatuh
    function createHeart() {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.innerHTML = "❤️";

      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (3 + Math.random() * 5) + "s";
      heart.style.fontSize = (15 + Math.random() * 20) + "px";

      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 8000);
    }

    setInterval(createHeart, 300);
  </script>

</body>
</html>
