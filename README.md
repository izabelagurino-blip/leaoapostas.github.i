<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>LEÃO APOSTAS • Gerador</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family: 'Segoe UI', Arial, sans-serif;
}

body{
  background: radial-gradient(circle at top, #1a1a1a, #000);
  color:#fff;
  min-height:100vh;
}

header{
  padding:25px;
  text-align:center;
}

header h1{
  color:#f5a623;
  font-size:2.2rem;
}

header p{
  opacity:.8;
  margin-top:8px;
}

.container{
  max-width:420px;
  margin:40px auto;
  background:rgba(255,255,255,0.05);
  backdrop-filter: blur(10px);
  border-radius:15px;
  padding:25px;
  box-shadow:0 0 25px rgba(0,0,0,.6);
}

label{
  display:block;
  margin:15px 0 5px;
  font-size:.9rem;
  opacity:.85;
}

select, button{
  width:100%;
  padding:12px;
  border-radius:8px;
  border:none;
  font-size:1rem;
}

select{
  background:#111;
  color:#fff;
}

button{
  margin-top:20px;
  background:linear-gradient(135deg,#f5a623,#ffcc70);
  color:#000;
  font-weight:bold;
  cursor:pointer;
  transition:.3s;
}

button:hover{
  transform:scale(1.03);
}

.resultado{
  margin-top:25px;
  padding:15px;
  border-radius:10px;
  background:#0d0d0d;
  text-align:center;
  display:none;
}

.resultado h2{
  color:#f5a623;
  margin-bottom:10px;
}

footer{
  text-align:center;
  margin-top:40px;
  font-size:.85rem;
  opacity:.6;
}
</style>
</head>

<body>

<header>
  <h1>🦁 LEÃO APOSTAS</h1>
  <p>Gerador Profissional de Sensibilidade</p>
</header>

<div class="container">

  <label>Marca do celular</label>
  <select id="marca">
    <option value="">Selecione</option>
    <option>Apple</option>
    <option>Samsung</option>
    <option>Xiaomi</option>
    <option>Motorola</option>
    <option>Asus</option>
    <option>Realme</option>
    <option>Infinix</option>
    <option>LG</option>
  </select>

  <label>Modelo</label>
  <select id="modelo">
    <option value="">Selecione</option>
    <option>Entrada</option>
    <option>Intermediário</option>
    <option>Top de Linha</option>
  </select>

  <button onclick="gerar()">GERAR SENSI 🔥</button>

  <div class="resultado" id="res">
    <h2>Sensibilidade Gerada</h2>
    <p id="texto"></p>
  </div>

</div>

<footer>
  © LEÃO APOSTAS • Org Oficial
</footer>

<script>
function gerar(){
  const marca = document.getElementById("marca").value;
  const modelo = document.getElementById("modelo").value;
  const res = document.getElementById("res");
  const texto = document.getElementById("texto");

  if(!marca || !modelo){
    alert("Selecione marca e modelo!");
    return;
  }

  const geral = Math.floor(Math.random()*40)+160;
  const redDot = Math.floor(Math.random()*30)+140;
  const mira2x = Math.floor(Math.random()*30)+130;
  const mira4x = Math.floor(Math.random()*30)+120;
  const awm = Math.floor(Math.random()*25)+100;

  texto.innerHTML = `
    📱 <b>${marca}</b> (${modelo})<br><br>
    🎯 Geral: <b>${geral}</b><br>
    🔴 Red Dot: <b>${redDot}</b><br>
    🔭 2x: <b>${mira2x}</b><br>
    🔍 4x: <b>${mira4x}</b><br>
    🎯 AWM: <b>${awm}</b>
  `;

  res.style.display = "block";
}
</script>

</body>
</html>
