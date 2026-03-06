<!DOCTYPE html>
<html lang="hu">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Boldog Nőnapot!</title>
<style>
body{
font-family: Arial, sans-serif;
background: linear-gradient(135deg,#ff9a9e,#fad0c4);
margin:0;
height:100vh;
display:flex;
align-items:center;
justify-content:center;
color:#333;
}
.card{
background:white;
padding:40px;
border-radius:20px;
box-shadow:0 10px 30px rgba(0,0,0,0.2);
text-align:center;
max-width:500px;
}
h1{
font-size:36px;
margin-bottom:10px;
}
.message{
font-size:18px;
margin:20px 0;
line-height:1.6;
}
button{
background:#ff6b81;
border:none;
color:white;
padding:12px 24px;
font-size:16px;
border-radius:10px;
cursor:pointer;
}
button:hover{
background:#ff4f6d;
}
.hidden{
display:none;
margin-top:20px;
}
img{
max-width:100%;
border-radius:15px;
margin-top:15px;
}
</style>
</head>
<body>

<div class="card">
<h1>Boldog Nőnapot! 🌸</h1>
<div class="message">
Szerettem volna valami apró meglepetést küldeni neked,
még akkor is, ha most messze vagyunk egymástól.
</div>

<button onclick="showMessage()">Kattints ide ❤️</button>

<div id="secret" class="hidden">
<p>Te vagy az egyik legkülönlegesebb ember az életemben. 💕</p>

<img src="kep.jpeg" alt="Közös képünk">

<audio id="music" controls>
  <source src="zene.mp3" type="audio/mpeg">
  A böngésződ nem támogatja az audio lejátszást.
</audio>

</div>
</div>

<script>
function showMessage(){
const secret = document.getElementById('secret');
secret.style.display='block';

const music = document.getElementById('music');
music.play();
}
</script>

</body>
</html>
