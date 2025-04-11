<!DOCTYPE html>
<html>
<head>
  <title>For Amore K</title>
  <style>
    body {
      background-color: #ffe6f0;
      color: #ff4d94;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      text-align: center;
      margin-top: 80px;
      overflow: hidden;
    }

    h1 {
      font-size: 50px;
      animation: bounce 1s infinite alternate;
    }

    p {
      font-size: 22px;
      color: #ff66b2;
      margin-top: 20px;
    }

    button {
      background-color: #ffb3d9;
      color: white;
      border: none;
      padding: 15px 30px;
      font-size: 20px;
      border-radius: 20px;
      cursor: pointer;
      box-shadow: 0 6px 8px rgba(0,0,0,0.1);
      transition: 0.3s;
      margin-top: 30px;
    }

    button:hover {
      background-color: #ff80bf;
      transform: scale(1.1);
    }

    #surprise {
      margin-top: 30px;
      font-size: 24px;
      display: none;
      animation: fadeIn 1s ease-in-out;
      color: #ff4d94;
    }

    #iMissYouButton {
      display: none;
      background-color: #ff80bf;
      color: white;
      padding: 15px 30px;
      font-size: 22px;
      border-radius: 20px;
      cursor: pointer;
      margin-top: 20px;
      animation: fadeIn 1s ease-in-out;
    }

    .sparkle-heart {
      font-size: 50px;
      animation: heartBeat 1s infinite alternate, sparkle 1.5s infinite alternate;
      color: #ff66b2;
    }

    .sparkle {
      position: absolute;
      animation: sparkleEffect 1.5s infinite;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes heartBeat {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.2);
      }
      100% {
        transform: scale(1);
      }
    }

    @keyframes sparkleEffect {
      0% {
        transform: scale(1) rotate(0);
        opacity: 0;
      }
      100% {
        transform: scale(1.5) rotate(360deg);
        opacity: 1;
      }
    }

    @keyframes sparkle {
      0% {
        transform: translate(0, 0);
      }
      50% {
        transform: translate(20px, 20px);
      }
      100% {
        transform: translate(-20px, -20px);
      }
    }

    @keyframes bounce {
      0% {
        transform: translateY(0);
      }
      100% {
        transform: translateY(-10px);
      }
    }

  </style>
</head>
<body>

  <h1>Hi, Amore K!</h1>
  <p>This page is made just for you 💖</p>
  <button onclick="showLove()">Click Me!</button>

  <div id="surprise">
    <p>Every day with you is a reminder of how lucky I am. You bring so much light into my life, and I feel so blessed to have you by my side. Your laughter, your kindness, your love, and your amazing heart make every moment we share feel like a treasure. 💕</p>
    <p>Even when things get tough, I know we can face them together. You are my joy, my comfort, and my everything. Every little thing you do, from the way you smile to the way you care for those around you, makes me fall in love with you more and more each day. 💖</p>
    <p>Thank you for being you, for being my amazing Amore K. You make the world a better place just by being in it, and I’ll always cherish and adore you. 💕</p>
    <div class="sparkle-heart">💖</div>
    <div class="sparkle" style="top: 70px; left: 100px;">✨</div>
    <div class="sparkle" style="top: 120px; left: 180px;">✨</div>
    <div class="sparkle" style="top: 160px; left: 50px;">✨</div>
  </div>

  <button id="iMissYouButton" onclick="showMissYouMessage()">I Miss Youuuu!</button>

  <script>
    function showLove() {
      document.getElementById("surprise").style.display = "block";
      document.getElementById("surprise").classList.add("fadeIn");
      document.getElementById("iMissYouButton").style.display = "inline-block"; // Show the "I Miss Youuuu" button
    }

    function showMissYouMessage() {
      alert("I miss you soooo much! 💖💖 Can't wait to see you soon!");
    }
  </script>

</body>
</html>
