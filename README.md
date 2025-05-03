<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <title>Login - ENHYPEN</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: url("ENHYPENLOGINN.jpg") no-repeat center center fixed;
      background-size: cover;
      color: #f4f4f4;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .login-container {
      background: rgba(0, 0, 0, 0.65);
      padding: 40px;
      border-radius: 15px;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
      width: 400px;
      text-align: center;
    }

    .login-container h1 {
      color: #ffcc70;
      margin-bottom: 30px;
      font-size: 28px;
    }

    .form-group {
      margin-bottom: 25px;
      text-align: left;
    }

    .form-group label {
      display: block;
      margin-bottom: 8px;
      font-weight: bold;
    }

    .form-group input {
      width: 100%;
      padding: 12px;
      border: 2px solid rgba(255, 204, 112, 0.3);
      border-radius: 8px;
      background: rgba(255, 255, 255, 0.1);
      color: #fff;
      font-size: 16px;
      transition: all 0.3s;
    }

    .form-group input:focus {
      outline: none;
      border-color: #ffcc70;
      background: rgba(255, 255, 255, 0.2);
    }

    .login-btn {
      width: 100%;
      padding: 12px;
      background: #ffcc70;
      color: #000;
      border: none;
      border-radius: 8px;
      font-weight: bold;
      cursor: pointer;
      transition: all 0.3s;
      font-size: 16px;
      margin-top: 15px;
    }

    .login-btn:hover {
      background: #ffd787;
      transform: translateY(-2px);
    }
  </style>
</head>
<body>
  <div class="login-container">
    <h1>Login ENHYPEN FANS</h1>
    <form id="loginForm">
      <div class="form-group">
        <label for="username">Username</label>
        <input type="text" id="username" name="username" required>
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" name="password" required>
      </div>
      <button type="submit" class="login-btn">LOGIN</button>
    </form>
  </div>

  <script>
    document.getElementById('loginForm').addEventListener('submit', function(e) {
      e.preventDefault();
      
      const username = document.getElementById('username').value;
      const password = document.getElementById('password').value;
      
      // Validasi sederhana
      if(username && password) {
        // Redirect ke halaman utama setelah login berhasil
        window.location.href = 'halaman1.html';
      } else {
        alert('Silakan isi username dan password!');
      }
    });
  </script>
</body>
</html>
