# Rose-day-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For You ❤️</title>

<link rel="icon" href="https://c4.wallpaperflare.com/wallpaper/812/187/770/kimi-no-na-wa-tachibana-taki-miyamizu-mitsuha-anime-wallpaper-preview.jpg">

<link href="https://fonts.googleapis.com/css2?family=Great+Vibes&display=swap" rel="stylesheet">

<style>
body, html {
    margin: 0;
    padding: 0;
    height: 100%;
    width: 100%;
    font-family: 'Great Vibes', cursive;
    background: linear-gradient(to right, #53efbe , #3b94ef);
    overflow: hidden;
}

/* Rose container */
.rose {
  position: absolute;
  width: 120px;
  height: 120px;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

/* Petals */
.petal {
  position: absolute;
  width: 60px;
  height: 60px;
  background: radial-gradient(circle at top left, #ff9aa2, #e6005c);
  border-radius: 50%;
  transform-origin: bottom right;
  animation: bloom 4s infinite ease-in-out;
}

.petal:nth-child(n) {
  transform: rotate(calc(var(--i) * 12deg));
}

/* Animation */
@keyframes bloom {
  0%,100% { transform: scale(1) rotate(var(--r)); }
  50% { transform: scale(1.15) rotate(var(--r)); }
}

/* Text in center */
.text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: white;
  z-index: 10;
}

.text span {
  font-size: 28px;
  display: block;
}

#prompt {
  position: absolute;
  top: 65%;
  width: 100%;
  text-align: center;
  font-family: monospace;
  color: #fff;
  font-size: 14px;
}

/* Footer */
h1 {
  position: absolute;
  bottom: 10px;
  right: 15px;
  font-size: 14px;
  font-family: monospace;
}

a {
  color: #fff;
  text-decoration: none;
  font-family: monospace;
}
</style>
</head>

<body>

<div class="rose">
  <!-- 30 petals -->
  <script>
    for(let i=0;i<30;i++){
      document.write(`<div class="petal" style="--i:${i}; --r:${i*12}deg;"></div>`);
    }
  </script>

  <div class="text">
    <span>Happy Rose Day 🌹</span>
    <span>My Darling ❤️✨</span>
  </div>
</div>

<span id="prompt">Touch the rose 💫</span>

<audio autoplay loop>
  <source src="https://heyyouu.netlify.app/song.mp3" type="audio/mp3">
</audio>

<h1>By your one & only 😌✨</h1>

</body>
</html>
