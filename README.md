<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sameer Pasha</title>
  <style>
    @keyframes gradientText {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    @keyframes snowflakes-fall {
      0% { top: -10%; }
      100% { top: 100%; }
    }

    @keyframes snowflakes-shake {
      0% { transform: translateX(0px); }
      50% { transform: translateX(80px); }
      100% { transform: translateX(0px); }
    }

    .neon-heading {
      font-family: 'Inter', sans-serif;
      margin: 0;
      font-size: 4em;
      font-weight: 900;
      letter-spacing: -.05em;
      text-align: center;
      background: linear-gradient(270deg, #39ff14, #00ff99);
      background-size: 200%;
      background-clip: text;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: gradientText 3s ease infinite;
    }

    .snowflake {
      color: #fff;
      font-size: 1em;
      font-family: Arial;
      text-shadow: 0 0 1px #000;
      position: fixed;
      top: -10%;
      z-index: 9999;
      user-select: none;
      pointer-events: none;
      animation-name: snowflakes-fall, snowflakes-shake;
      animation-duration: 10s, 3s;
      animation-timing-function: linear, ease-in-out;
      animation-iteration-count: infinite, infinite;
    }

    .snowflake:nth-of-type(1) { left: 5%; animation-delay: 0s, 0s; }
    .snowflake:nth-of-type(2) { left: 15%; animation-delay: 1s, 1s; }
    .snowflake:nth-of-type(3) { left: 25%; animation-delay: 2s, 0.5s; }
    .snowflake:nth-of-type(4) { left: 35%; animation-delay: 3s, 2s; }
    .snowflake:nth-of-type(5) { left: 50%; animation-delay: 4s, 1s; }
    .snowflake:nth-of-type(6) { left: 65%; animation-delay: 5s, 1.5s; }
    .snowflake:nth-of-type(7) { left: 75%; animation-delay: 6s, 2.5s; }
    .snowflake:nth-of-type(8) { left: 85%; animation-delay: 7s, 0.5s; }
    .snowflake:nth-of-type(9) { left: 95%; animation-delay: 8s, 2s; }
  </style>
</head>
<body>
  <h1 class="neon-heading">Sameer Pasha</h1>
  <div class="snowflake">❅</div>
  <div class="snowflake">❅</div>
  <div class="snowflake">❅</div>
  <div class="snowflake">❅</div>
  <div class="snowflake">❅</div>
  <div class="snowflake">❅</div>
  <div class="snowflake">❅</div>
  <h1>Hi 👋, I'm Sameer Pasha</h1>
  <p>A passionate Artificial intelligence and Machine learning engineer</p>
  <h2>🚀 Languages and Tools I Use</h2>
  <p><!-- ICON LINKS AS IN USER INPUT (omitted for brevity) --></p>
  <h2>✍️ Recent Posts</h2>
  <ul>
    <li><a target="_blank" href="https://github.com/sameerpashaaa/SiteSnapper">I created a tool that gets you the front end info of any website just by entering its URL.</a></li>
  </ul>
  <h2>⚡️ Where to find me</h2>
  <p><!-- SOCIAL BADGES AS IN USER INPUT (omitted for brevity) --></p>
  <p><img align="center" src="https://github-readme-stats.vercel.app/api?username=sameerpashaaa&show_icons=true&locale=en" alt="sameerpashaaa" /></p>
  <p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=sameerpashaaa&" alt="sameerpashaaa" /></p>
  <p><a href="https://github.com/ryo-ma/github-profile-trophy"><img src="https://github-profile-trophy.vercel.app/?username=sameerpashaaa" alt="sameerpashaaa" /></a></p>
</body>
</html>
