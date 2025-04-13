<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Form Cinta khusus untuk bibil 💌</title>
  <style>
    body {
      font-family: 'Comic Sans MS', cursive;
      background: linear-gradient(to right, #ff9a9e, #fad0c4);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    .form-container {
      background: white;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 5px 20px rgba(0,0,0,0.1);
      width: 350px;
      text-align: center;
    }

    h2 {
      color: #ff4d6d;
      margin-bottom: 20px;
    }

    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }

    input[type="text"],
    textarea,
    select {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 8px;
    }

    button {
      margin-top: 20px;
      background-color: #ff4d6d;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }

    button:hover {
      background-color: #e63950;
    }

    .thanks-message {
      display: none;
      color: green;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div class="form-container">
    <h2>💘 Untuk Kamu Sengg 💘</h2>
    <form id="loveForm">
      <label for="sayang">Seberapa kamu sayang aku?</label>
      <select id="sayang" name="sayang">
        <option value="banget">Banget Banget! 💖</option>
        <option value="banget">Banget! 😍</option>
        <option value="biasa">Biasa aja... (bohong ya?) 😅</option>
      </select>

      <label for="kapan">Kapan kita ngopi?</label>
      <input type="text" id="kapan" name="kapan" placeholder="Misalnya: Minggu depan ❤️">

      <label for="pesan">Pesan manis buat aku 💌</label>
      <textarea id="pesan" name="pesan" rows="4" placeholder="Tulis pesanmu di sini..."></textarea>

      <button type="submit">Kirim 💌</button>
      <p class="thanks-message" id="thanksMsg">Terima kasih Sengg! 💕</p>
    </form>
  </div>

  <script>
    document.getElementById('loveForm').addEventListener('submit', function(e) {
      e.preventDefault(); // Biar gak reload
      document.getElementById('thanksMsg').style.display = 'block';
    });
  </script>
</body>
</html>
