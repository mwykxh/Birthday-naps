<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday Nani 💖</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      background: linear-gradient(-45deg, #ff9a9e, #fad0c4, #fbc2eb, #a18cd1);
      background-size: 400% 400%;
      animation: gradientBG 12s ease infinite;
      font-family: "Poppins", sans-serif;
      overflow: hidden;
    }@keyframes gradientBG {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

h1 {
  font-size: 3rem;
  color: #fff;
  text-shadow: 0 0 20px rgba(255, 0, 120, 0.8);
  animation: glow 2s ease-in-out infinite alternate;
  text-align: center;
  margin: 0;
}

@keyframes glow {
  from { text-shadow: 0 0 10px #ff69b4, 0 0 20px #ff69b4; }
  to { text-shadow: 0 0 20px #ff1493, 0 0 40px #ff1493; }
}

h2 {
  font-size: 1.5rem;
  color: #fff;
  margin-top: 15px;
  animation: fadeIn 3s ease forwards;
  opacity: 0;
}

.message {
  margin-top: 25px;
  padding: 15px 25px;
  background: rgba(255, 255, 255, 0.15);
  border-radius: 15px;
  color: #fff;
  font-size: 1.2rem;
  text-align: center;
  animation: fadeIn 5s ease forwards;
  opacity: 0;
  backdrop-filter: blur(4px);
}

@keyframes fadeIn {
  to { opacity: 1; }
}

.heart {
  position: absolute;
  width: 20px;
  height: 20px;
  background: red;
  transform: rotate(45deg);
  animation: float 6s linear infinite;
  bottom: -20px;
}

.heart::before, .heart::after {
  content: '';
  position: absolute;
  width: 20px;
  height: 20px;
  background: red;
  border-radius: 50%;
}

.heart::before { top: -10px; left: 0; }
.heart::after { left: -10px; top: 0; }

@keyframes float {
  0% { transform: translateY(0) rotate(45deg); opacity: 1; }
  100% { transform: translateY(-800px) rotate(45deg); opacity: 0; }
}

#overlay {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.7);
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  z-index: 10;
}

#overlay button {
  padding: 12px 25px;
  font-size: 1.2rem;
  border: none;
  border-radius: 30px;
  background: #ff4b8b;
  color: white;
  cursor: pointer;
  box-shadow: 0 0 15px rgba(0,0,0,0.4);
  transition: transform 0.2s;
}

#overlay button:hover { transform: scale(1.1); }

  </style>
</head>
<body>
  <div id="overlay">
    <h2 style="color:white; margin-bottom:20px;">Tap to start the surprise 🎁</h2>
    <button onclick="startMusic()">Play Music 🎶</button>
  </div>  <h1>🎂 Happy Birthday Nani 💖</h1>
  <h2>Lots of love to you, Radha 🌹</h2>
  <div class="message">
    You are my world, my smile, and my forever. <br />
    Wishing you the happiest birthday, my dearest Nani! 💝
  </div>  <audio id="bgm" loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_5bfb0b72e6.mp3?filename=romantic-piano-11364.mp3" type="audio/mpeg" />
  </audio>  <script>
    function createHeart() {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (3 + Math.random() * 5) + 's';
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 8000);
    }
    setInterval(createHeart, 400);

    function startMusic() {
      document.getElementById('bgm').play();
      document.getElementById('overlay').style.display = 'none';
    }
  </script></body>
</html>

# Birthday-naps
I love you..💋🎈🎂
