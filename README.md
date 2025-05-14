<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Neon Name Rain</title>
  <style>
    body {
      background: black;
      margin: 0;
      overflow: hidden;
    }
    canvas {
      display: block;
    }
  </style>
</head>
<body>
<canvas id="matrix"></canvas>
<script>
  const canvas = document.getElementById("matrix");
  const ctx = canvas.getContext("2d");

  // Fullscreen canvas
  canvas.height = window.innerHeight;
  canvas.width = window.innerWidth;

  // Letters to use
  const letters = "A L E X".split(""); // Change to your name or any letters
  const fontSize = 20;
  const columns = canvas.width / fontSize;

  // Drops per column
  const drops = Array(Math.floor(columns)).fill(1);

  function draw() {
    // Black background with low opacity for trailing effect
    ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
    ctx.fillRect(0, 0, canvas.width, canvas.height);

    ctx.font = fontSize + "px monospace";

    for (let i = 0; i < drops.length; i++) {
      const text = letters[Math.floor(Math.random() * letters.length)];
      ctx.fillStyle = `hsl(${Math.random() * 360}, 100%, 70%)`; // Neon random colors
      ctx.fillText(text, i * fontSize, drops[i] * fontSize);

      if (drops[i] * fontSize > canvas.height || Math.random() > 0.95) {
        drops[i] = 0;
      }
      drops[i]++;
    }
  }

  setInterval(draw, 33);
</script>
</body>
</html>
