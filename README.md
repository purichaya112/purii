<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ถึงบิบี๋ 💗</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Prompt', sans-serif;
      background: linear-gradient(135deg, #ffe1f0, #d5f0ff);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
      color: #ff4d88;
      text-align: center;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5em;
    }

    p {
      font-size: 1.2rem;
      max-width: 80%;
      margin: 0 auto;
    }

    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: #ff4d88;
      transform: rotate(45deg);
      animation: float 6s infinite ease-in-out;
    }

    .heart::before,
    .heart::after {
      content: "";
      position: absolute;
      width: 20px;
      height: 20px;
      background: #ff4d88;
      border-radius: 50%;
    }

    .heart::before {
      top: -10px;
      left: 0;
    }

    .heart::after {
      left: -10px;
      top: 0;
    }

    @keyframes float {
      0% {
        bottom: -20px;
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        bottom: 100%;
        left: calc(100vw * var(--x));
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div>
    <h1>I have somethings to tell u ,bab💗</h1>
    <p>Happy 1st month with you~<br>You are the first person i want to see in the morning and
you are the last person I want to see before I go to bed.💕</p>
  </div>

  <!-- หัวใจลอยๆ -->
  <script>
    for (let i = 0; i < 30; i++) {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.setProperty('--x', Math.random());
      heart.style.animationDelay = Math.random() * 5 + "s";
      document.body.appendChild(heart);
    }
  </script>
</body>
</html>
