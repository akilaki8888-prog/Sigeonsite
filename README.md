# Sigeonsite
A Funny site frkm pigeons ai category!
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sogeon Hub</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #eaf7ff, #ffffff);
      color: #222;
      min-height: 100vh;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 18px 25px;
      background: white;
      box-shadow: 0 2px 10px #0002;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .logo {
      font-size: 25px;
      font-weight: bold;
    }

    nav button {
      border: 0;
      background: #eee;
      padding: 10px 15px;
      margin-left: 6px;
      border-radius: 10px;
      cursor: pointer;
      font-weight: bold;
    }

    nav button:hover {
      background: #ddd;
    }

    main {
      text-align: center;
      padding: 70px 20px;
    }

    .title {
      font-size: clamp(40px, 9vw, 80px);
      font-weight: 900;
      margin: 0;
      letter-spacing: 4px;
    }

    .title span {
      display: inline-block;
      animation: letterBounce 1.5s infinite;
    }

    .title span:nth-child(2) { animation-delay: .1s; }
    .title span:nth-child(3) { animation-delay: .2s; }
    .title span:nth-child(4) { animation-delay: .3s; }
    .title span:nth-child(5) { animation-delay: .4s; }
    .title span:nth-child(6) { animation-delay: .5s; }
    .title span:nth-child(7) { animation-delay: .6s; }
    .title span:nth-child(8) { animation-delay: .7s; }
    .title span:nth-child(9) { animation-delay: .8s; }
    .title span:nth-child(10) { animation-delay: .9s; }

    @keyframes letterBounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    .pigeon-area {
      height: 150px;
      position: relative;
      overflow: hidden;
      margin-top: 30px;
    }<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sogeon Hub</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #eaf7ff, #ffffff);
      color: #222;
      min-height: 100vh;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 18px 25px;
      background: white;
      box-shadow: 0 2px 10px #0002;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .logo {
      font-size: 25px;
      font-weight: bold;
    }

    nav button {
      border: 0;
      background: #eee;
      padding: 10px 15px;
      margin-left: 6px;
      border-radius: 10px;
      cursor: pointer;
      font-weight: bold;
    }

    nav button:hover {
      background: #ddd;
    }

    main {
      text-align: center;
      padding: 70px 20px;
    }

    .title {
      font-size: clamp(40px, 9vw, 80px);
      font-weight: 900;
      margin: 0;
      letter-spacing: 4px;
    }

    .title span {
      display: inline-block;
      animation: letterBounce 1.5s infinite;
    }

    .title span:nth-child(2) { animation-delay: .1s; }
    .title span:nth-child(3) { animation-delay: .2s; }
    .title span:nth-child(4) { animation-delay: .3s; }
    .title span:nth-child(5) { animation-delay: .4s; }
    .title span:nth-child(6) { animation-delay: .5s; }
    .title span:nth-child(7) { animation-delay: .6s; }
    .title span:nth-child(8) { animation-delay: .7s; }
    .title span:nth-child(9) { animation-delay: .8s; }
    .title span:nth-child(10) { animation-delay: .9s; }

    @keyframes letterBounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    .pigeon-area {
      height: 150px;
      position: relative;
      overflow: hidden;
      margin-top: 30px;
    }

    .pigeon {
      position: absolute;
      left: -120px;
      bottom: 20px;
      font-size: 75px;
      animation: walkPigeon 10s linear infinite;
    }

    @keyframes walkPigeon {
      0% {
        left: -120px;
        transform: scaleX(1);
      }

      48% {
        left: 80%;
        transform: scaleX(1);
      }

      52% {
        left: 80%;
        transform: scaleX(-1);
      }

      100% {
        left: -120px;
        transform: scaleX(-1);
      }
    }

    .card {
      max-width: 500px;
      margin: 30px auto;
      padding: 30px;
      background: white;
      border-radius: 20px;
      box-shadow: 0 5px 25px #0002;
    }

    input {
      width: 100%;
      padding: 13px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 10px;
      font-size: 16px;
    }

    .main-button {
      width: 100%;
      padding: 13px;
      margin-top: 10px;
      border: 0;
      border-radius: 10px;
      background: #222;
      color: white;
      font-size: 16px;
      cursor: pointer;
    }

    .main-button:hover {
      opacity: .85;
    }

    .settings {
      display: none;
    }

    .danger {
      background: #d33;
    }

    .admin {
      background: #555;
    }

    .message {
      margin-top: 15px;
      font-weight: bold;
    }
  </style>
</head>

<body>

  <header>
    <div class="logo">🐦 Sogeon Hub</div>

    <nav>
      <button onclick="showHome()">Home</button>
      <button onclick="showSettings()">⚙️ Settings</button>
      <button onclick="showAccount()">👤 Account</button>
    </nav>
  </header>

  <main>

    <!-- HOME -->
    <section id="home">

      <h1 class="title">
        <span>S</span><span>o</span><span>g</span><span>e</span><span>o</span><span>n</span>
        <span>H</span><span>u</span><span>b</span>
      </h1>

      <p>Welcome to Sogeon Hub!</p>

      <div class="pigeon-area">
        <div class="pigeon">🐦</div>
      </div>

      <div class="card">
        <h2>🏠 Home</h2>
        <p>Your new Sogeon Hub homepage.</p>
        <button class="main-button" onclick="showAccount()">
          Create a Free Account
        </button>
      </div>

    </section>


    <!-- ACCOUNT -->
    <section id="account" style="display:none;">

      <div class="card">

        <h2>👤 Create a Free Account</h2>

        <p>No Google or Apple account required.</p>

        <input id="username" type="text" placeholder="Choose a username">

        <input id="password" type="password" placeholder="Choose a password">

        <button class="main-button" onclick="createAccount()">
          Create Account
        </button>

        <div id="accountMessage" class="message"></div>

      </div>

    </section>


    <!-- SETTINGS -->
    <section id="settings" class="settings">

      <div class="card">

        <h2>⚙️ Settings</h2>

        <p id="currentUser">You are not logged in.</p>

        <button class="main-button admin" onclick="askAdmin()">
          👑 Ask the Owner for Admin
        </button>

        <button class="main-button danger" onclick="deleteAccount()">
          🗑️ Delete Account
        </button>

        <div id="settingsMessage" class="message"></div>

      </div>

    </section>

  </main>


  <script>

    function hideAll() {
      document.getElementById("home").style.display = "none";
      document.getElementById("account").style.display = "none";
      document.getElementById("settings").style.display = "none";
    }

    function showHome() {
      hideAll();
      document.getElementById("home").style.display = "block";
    }

    function showAccount() {
      hideAll();
      document.getElementById("account").style.display = "block";
    }

    function showSettings() {
      hideAll();
      document.getElementById("settings").style.display = "block";

      const username = localStorage.getItem("sogeonUsername");

      if (username) {
        document.getElementById("currentUser").textContent =
          "Logged in as: " + username;
      } else {
        document.getElementById("currentUser").textContent =
          "You are not logged in.";
      }
    }

    function createAccount() {

      const username = document.getElementById("username").value.trim();
      const password = document.getElementById("password").value;

      const message = document.getElementById("accountMessage");

      if (username.length < 3) {
        message.textContent = "Username must be at least 3 characters.";
        return;
      }

      if (password.length < 4) {
        message.textContent = "Password must be at least 4 characters.";
        return;
      }

      localStorage.setItem("sogeonUsername", username);

      message.textContent =
        "Account created! Welcome, " + username + " 🎉";

      document.getElementById("username").value = "";
      document.getElementById("password").value = "";
    }

    function deleteAccount() {

      const username = localStorage.getItem("sogeonUsername");

      if (!username) {
        document.getElementById("settingsMessage").textContent =
          "You don't have an account saved on this device.";
        return;
      }

      const confirmed = confirm(
        "Delete your Sogeon Hub account?"
      );

      if (confirmed) {

        localStorage.removeItem("sogeonUsername");

        document.getElementById("currentUser").textContent =
          "Account deleted.";

        document.getElementById("settingsMessage").textContent =
          "Your local demo account has been deleted.";
      }
    }

    function askAdmin() {

      const username = localStorage.getItem("sogeonUsername");

      if (!username) {
        alert("Create an account first.");
        return;
      }

      alert(
        "Admin request sent for " +
        username +
        " 👑"
      );
    }

  </script>

</body>
</html>
