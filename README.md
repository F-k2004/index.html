<!-- ndex.html -->
<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <title>وب‌سایت من</title>
  <style>
    body {
      font-family: sans-serif;
      text-align: center;
      background: linear-gradient(135deg, #74ebd5, #ACB6E5);
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
    h1 {
      color: #333;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      margin-top: 20px;
      cursor: pointer;
      border: none;
      border-radius: 8px;
      background-color: #ff7b54;
      color: white;
      transition: 0.3s;
    }
    button:hover {
      background-color: #ff3d00;
    }
    p {
      margin-top: 20px;
      font-size: 18px;
      color: #222;
    }
  </style>
</head>
<body>
  <h1>👋 به وب‌سایت من خوش آمدید!</h1>
  <button onclick="showMessage()">نمایش پیام</button>
  <p id="message"></p>

  <script>
    const messages = [
      "✨ امروز بهترین روز برای شروعه!",
      "🚀 با هر قدم، به هدفت نزدیک‌تر می‌شی.",
      "🌱 هر چالش فرصتی برای رشد است.",
      "🔥 تو توانایی انجامش رو داری!"
    ];

    function showMessage() {
      const msg = messages[Math.floor(Math.random() * messages.length)];
      document.getElementById("message").textContent = msg;
    }
  </script>
</body>
</html>
