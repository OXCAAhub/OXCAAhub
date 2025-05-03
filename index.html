`login-dashboard.html`
```html
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" />
<title>Login Sistem Admin dan Anggota</title>
<style>
  /* Reset */
  * {
    box-sizing: border-box;
  }

  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    background: #1e2a38;
    color: #eee;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    padding: 1rem;
  }

  #app {
    background: #263544;
    border-radius: 12px;
    max-width: 350px;
    width: 100%;
    padding: 2rem 2rem 3rem 2rem;
    box-shadow: 0 8px 20px rgba(0,0,0,0.4);
    display: flex;
    flex-direction: column;
  }

  h1 {
    margin: 0 0 1.5rem 0;
    font-size: 1.8rem;
    font-weight: 700;
    color: #4cd137;
    text-align: center;
  }

  form {
    display: flex;
    flex-direction: column;
  }

  label {
    margin-bottom: 0.3rem;
    font-weight: 600;
  }

  input[type="text"], input[type="password"] {
    padding: 0.7rem;
    border-radius: 8px;
    border: none;
    font-size: 1rem;
    margin-bottom: 1.2rem;
    outline: none;
  }

  input[type="text"]:focus, input[type="password"]:focus {
    outline: 2px solid #4cd137;
  }

  button {
    background-color: #44bd32;
    color: white;
    border: none;
    border-radius: 8px;
    padding: 0.75rem;
    font-size: 1.1rem;
    font-weight: 700;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  button:hover {
    background-color: #2f8706;
  }

  .error {
    color: #ff6b6b;
    font-weight: 600;
    margin-bottom: 1rem;
    text-align: center;
  }

  .welcome {
    text-align: center;
    margin-bottom: 1rem;
    font-size: 1.2rem;
    font-weight: 600;
    color: #4cd137;
  }

  .saldo {
    font-size: 1.4rem;
    font-weight: 700;
    color: #fbc531;
    text-align: center;
    margin-bottom: 1.5rem;
  }

  .menu {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }

  .menu button {
    background-color: #273c75;
    border-radius: 8px;
    padding: 0.8rem;
    font-size: 1rem;
    font-weight: 600;
    cursor: pointer;
    color: #f5f6fa;
    border: 2px solid transparent;
    transition: background-color 0.3s ease, border-color 0.3s ease;
    text-align: center;
  }

  .menu button:hover {
    background-color: #4cd137;
    border-color: #27ae60;
    color: #1e272e;
  }

  .logout-btn {
    margin-top: 2rem;
    background-color: #e84118;
  }

  .logout-btn:hover {
    background-color: #c23616;
  }

  @media (max-width: 400px) {
    #app {
      padding: 1.5rem 1.5rem 2rem 1.5rem;
    }
    h1 {
      font-size: 1.5rem;
    }
  }
</style>
</head>
<body>
<div id="app" role="main" aria-live="polite">

  <!-- Login Form -->
  <form id="loginForm" aria-label="Form login dengan username dan key">
    <h1>Login Sistem</h1>
    <div class="error" id="errorMsg" role="alert" aria-live="assertive" style="display:none;"></div>
    <label for="username">Username</label>
    <input
      type="text"
      id="username"
      name="username"
      placeholder="A.BLACK.id atau M.BLACK.id"
      autocomplete="username"
      required
      aria-required="true"
      aria-describedby="userHelp"
    />
    <div id="userHelp" style="font-size:0.8rem; margin-top:-0.8rem; margin-bottom:1rem; color:#bcd4e6;">
      Format username: A.BLACK.id (admin) atau M.BLACK.id (anggota)
    </div>

    <label for="key">Key</label>
    <input
      type="password"
      id="key"
      name="key"
      placeholder="Masukkan Key"
      autocomplete="current-password"
      required
      aria-required="true"
    />

    <button type="submit" aria-label="Submit login">Masuk</button>
  </form>

  <!-- Dashboard -->
  <section id="dashboard" style="display:none;">
    <h1>Dashboard</h1>
    <div class="welcome" id="welcomeMsg" aria-live="polite"></div>
    <div class="saldo" id="saldoDisplay" aria-label="Saldo tersedia"></div>
    <div class="menu" role="list" aria-label="Menu metode kebutuhan">
      <button role="listitem" aria-label="Top Up Keperluan Anak" onclick="alert('Metode: Top Up Keperluan Anak')">Top Up Keperluan Anak</button>
      <button role="listitem" aria-label="JB Transfer" onclick="alert('Metode: JB Transfer')">JB Transfer</button>
      <button role="listitem" aria-label="Isi Saldo" onclick="alert('Metode: Isi Saldo')">Isi Saldo</button>
      <button role="listitem" aria-label="Metode Lainnya" onclick="alert('Metode: Lainnya')">Metode Lainnya</button>
    </div>
    <button class="logout-btn" aria-label="Logout" onclick="logout()">Logout</button>
  </section>

</div>

<script>
  (function(){
    const loginForm = document.getElementById('loginForm');
    const errorMsg = document.getElementById('errorMsg');
    const dashboard = document.getElementById('dashboard');
    const welcomeMsg = document.getElementById('welcomeMsg');
    const saldoDisplay = document.getElementById('saldoDisplay');
    const app = document.getElementById('app');

    // Credentials data (example)
    // Since no backend, we hardcode valid usernames and key combination for demo
    // Key for all users is '001235', username either starting with "A." or "M." with .BLACK.id suffix
    const VALID_KEY = '001235';

    function validateUsername(username) {
      // Username must match:
      // A.BLACK.id or M.BLACK.id, case insensitive
      return /^[AM]\.BLACK\.id$/i.test(username);
    }

    loginForm.addEventListener('submit', function(e) {
      e.preventDefault();
      errorMsg.style.display = 'none';
      const username = loginForm.username.value.trim();
      const key = loginForm.key.value.trim();

      if(!validateUsername(username)) {
        errorMsg.textContent = 'Username tidak valid. Format harus A.BLACK.id atau M.BLACK.id';
        errorMsg.style.display = 'block';
        loginForm.username.focus();
        return;
      }

      if(key !== VALID_KEY) {
        errorMsg.textContent = 'Key salah. Silakan periksa kembali.';
        errorMsg.style.display = 'block';
        loginForm.key.focus();
        return;
      }

      // Success login
      loginForm.style.display = 'none';
      dashboard.style.display = 'flex';

      const isAdmin = username.toUpperCase().startsWith('A.');

      welcomeMsg.textContent = `Selamat datang, ${isAdmin ? 'Admin' : 'Anggota'} ${username.toUpperCase()}`;
      if(isAdmin) {
        saldoDisplay.textContent = 'Saldo Anda: Rp 346.624.268';
      } else {
        // For anggota, show a placeholder saldo, assume smaller saldo
        saldoDisplay.textContent = 'Saldo Anda: Rp 1.250.000';
      }
    });

    window.logout = function() {
      dashboard.style.display = 'none';
      loginForm.style.display = 'flex';
      loginForm.username.value = '';
      loginForm.key.value = '';
      errorMsg.style.display = 'none';
      loginForm.username.focus();
      welcomeMsg.textContent = '';
      saldoDisplay.textContent = '';
    }
  })();
</script>
</body>
</html>

```
