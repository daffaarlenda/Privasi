<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
  body {
  background-image: url('https://files.catbox.moe/40aeja.jpg');
  background-size: cover;
  background-position: center;
}
    #output {
      background-color: cyan;
      border-radius: 20px;
      text-align: center;
    }

    #atas {
      background-color: yellow;
      border-radius: 20px;
      text-align: center;
    }

    .kotak-input {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 20px;
    }

     #inputBox, #email, #pw {
      background-color: #000;
      font-family: monospace;
      color: green;
      border-radius: 10px;
      padding: 10px;
      margin: 5px;
     }
     button {
       font-family: monospace;
       background-color: black;
       color: green;
       border-radius: 10px;
       padding: 10px;
       margin: 5px;
     }
  </style>
</head>
<body>

  <h1 id="output"></h1>
  <h1 id="atas"></h1>

  <div class="kotak-input">
    <input type="text" id="inputBox" placeholder="Masukkan sesuatu...">
    <label for="email">masukan email</label>
    <input type="email" id="email" placeholder="Masukkan email...">
    <label for="password">pw ne boloo</label>
    <input type="password" id="pw"
    placeholder="masukkan password"><br>
    <button onclick="cekPW()">selanjutnya</button>
  </div>

  <script>// Menyapa pengguna saat membuka halaman
let nama = prompt('Siapa nama Anda?');
document.getElementById("output").innerHTML = "Halo " + nama;
document.getElementById("atas").innerHTML = "Lagi apa, " + nama + "?";

// Fungsi untuk mengecek password
function cekPW(){
  let password = document.getElementById("pw").value;

  if (password === "codingan dapa") {
    // Jika password benar, pindah ke halaman lain
    window.location.href = "Dapit.html";
  } else {
    // Jika salah, tampilkan peringatan
    alert("Password salah, coba lagi.");
  }
}
</script>
  
</body>
</html>
