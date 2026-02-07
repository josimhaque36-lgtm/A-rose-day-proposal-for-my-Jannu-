# A-rose-day-proposal-for-my-Jannu-
For my Jann 😘
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Rose Day ❤️</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, sans-serif;
      background: linear-gradient(135deg, #ffd1dc, #fff0f5);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }.card {
  background: white;
  padding: 30px 40px;
  border-radius: 20px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.15);
  text-align: center;
  max-width: 360px;
  animation: pop 1s ease;
}

@keyframes pop {
  0% { transform: scale(0.7); opacity: 0; }
  100% { transform: scale(1); opacity: 1; }
}

h1 {
  color: #e63946;
  margin-bottom: 10px;
}

p {
  color: #444;
  font-size: 16px;
  line-height: 1.6;
}

.rose {
  font-size: 70px;
  margin: 15px 0;
  animation: float 2s infinite ease-in-out;
}

@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-10px); }
}

button {
  margin-top: 20px;
  background: #e63946;
  color: white;
  border: none;
  padding: 12px 25px;
  font-size: 16px;
  border-radius: 30px;
  cursor: pointer;
  transition: 0.3s;
}

button:hover {
  background: #c9182b;
  transform: scale(1.05);
}

.message {
  display: none;
  margin-top: 15px;
  font-weight: bold;
  color: #e63946;
  animation: fadeIn 1s ease;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

.hearts span {
  position: absolute;
  bottom: -20px;
  animation: rise 5s linear infinite;
  font-size: 20px;
  color: #ff6b81;
}

@keyframes rise {
  0% { transform: translateY(0); opacity: 1; }
  100% { transform: translateY(-110vh); opacity: 0; }
}

  </style>
</head>
<body>  <div class="card">
    <h1>Happy Rose Day 🌹</h1>
    <div class="rose">🌹</div>
    <p>
      Dear <strong>Sadia</strong>,<br />
      just like this rose,<br />
      my feelings for you are soft, pure,
      and grow more beautiful every day.
    </p>
    <p>Will you be mine? 💖</p>
    <button onclick="sayYes()">Yes 💌</button>
    <div id="msg" class="message">
      You just made my heart smile ❤️<br />
      Thank you for choosing me.
    </div>
  </div>  <div class="hearts"></div>  <script>
    function sayYes() {
      document.getElementById('msg').style.display = 'block';
    }

    const hearts = document.querySelector('.hearts');
    setInterval(() => {
      const heart = document.createElement('span');
      heart.innerHTML = '❤️';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = 3 + Math.random() * 3 + 's';
      hearts.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }, 300);
  </script></body>
</html>
