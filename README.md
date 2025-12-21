<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Junior Caps JR</title>

<style>
body {
  font-family: Arial, sans-serif;
  margin:0;
  padding:0;
  background:#f4f4f4;
}

header {
  background:#111;
  color:#fff;
  padding:20px;
  text-align:center;
}

header h1 { margin:0; }
header p { margin-top:5px; font-size:1rem; }

.catalogo {
  display:grid;
  grid-template-columns: repeat(auto-fit, minmax(180px,1fr));
  gap:15px;
  padding:20px;
  max-width:1200px;
  margin:auto;
}

.product {
  background:#fff;
  border-radius:10px;
  overflow:hidden;
  box-shadow:0 2px 5px rgba(0,0,0,0.2);
  transition:0.3s;
}

.product:hover { transform:translateY(-5px); }

.product img {
  width:100%;
  height:200px;
  object-fit:cover;
}

.p-body {
  padding:10px;
  text-align:center;
}

.p-title {
  font-weight:bold;
  margin-bottom:5px;
  font-size:1rem;
}

.price {
  margin-bottom:8px;
  font-weight:bold;
}

.btn {
  display:inline-block;
  padding:8px 12px;
  background:#25D366;
  color:#fff;
  text-decoration:none;
  border-radius:5px;
  transition:0.3s;
}

.btn:hover { background:#20b954; }

footer {
  text-align:center;
  padding:20px;
  background:#111;
  color:#fff;
}

footer a {
  color:#ffcc00;
  text-decoration:none;
}
</style>
</head>

<body>

<header>
  <h1>🧢 Junior Caps JR</h1>
  <p>Gorras estilo New Era calidad G5 - Venta al detalle y mayoreo</p>
</header>

<section class="catalogo">

  <article class="product">
    <img src="https://i.imgur.com/HLlskRP.jpg" alt="NY Classic Negro">
    <div class="p-body">
      <div class="p-title">NY Classic – Negro</div>
      <div class="price">$300 MXN</div>
      <a class="btn" href="#" onclick="comprar('NY Classic Negro'); return false;">Comprar</a>
    </div>
  </article>

  <article class="product">
    <img src="https://imgur.com/FwFlSJC.jpg" alt="31 NY Black">
    <div class="p-body">
      <div class="p-title">31 NY Black – Negro</div>
      <div class="price">$2,000 MXN</div>
      <a class="btn" href="#" onclick="comprar('31 NY Black Negro'); return false;">Comprar</a>
    </div>
  </article>

  <article class="product">
    <img src="https://imgur.com/dDoFbWn.jpg" alt="Barbas Galaxy">
    <div class="p-body">
      <div class="p-title">Barbas Galaxy – Negro</div>
      <div class="price">$2,000 MXN</div>
      <a class="btn" href="#" onclick="comprar('Barbas Galaxy Negro'); return false;">Comprar</a>
    </div>
  </article>

  <article class="product">
    <img src="https://imgur.com/2WIk8sw.jpg" alt="LA Clauds 31">
    <div class="p-body">
      <div class="p-title">LA Clauds 31 – Negro</div>
      <div class="price">$2,000 MXN</div>
      <a class="btn" href="#" onclick="comprar('LA Clauds 31 Negro'); return false;">Comprar</a>
    </div>
  </article>

  <article class="product">
    <img src="https://imgur.com/ygpFh1E.jpg" alt="Sad Boy DH">
    <div class="p-body">
      <div class="p-title">Sad Boy DH – Negro</div>
      <div class="price">$1,500 MXN</div>
      <a class="btn" href="#" onclick="comprar('Sad Boy DH Negro'); return false;">Comprar</a>
    </div>
  </article>

  <article class="product">
    <img src="https://imgur.com/LOTRkoR.jpg" alt="Rocstar CT">
    <div class="p-body">
      <div class="p-title">Rocstar CT – Negro</div>
      <div class="price">$1,600 MXN</div>
      <a class="btn" href="#" onclick="comprar('Rocstar CT Negro'); return false;">Comprar</a>
    </div>
  </article>

  <article class="product">
    <img src="https://imgur.com/hKV7oZN.jpg" alt="Chorme CT">
    <div class="p-body">
      <div class="p-title">Chorme CT – Negro</div>
      <div class="price">$1,600 MXN</div>
      <a class="btn" href="#" onclick="comprar('Chorme CT Negro'); return false;">Comprar</a>
    </div>
  </article>

</section>

<footer>
  <p>Síguenos en 
    <a href="https://www.instagram.com/junior_hats_jr" target="_blank">Instagram</a>
  </p>
</footer>

<!-- SCRIPT CLAVE PARA ANDROID + iOS -->
<script>
function comprar(producto) {
  const numero = "524428655081";
  const mensaje = "Hola, quiero comprar la gorra " + producto;
  const url = "https://wa.me/" + numero + "?text=" + encodeURIComponent(mensaje);
  window.open(url, "_blank");
}
</script>

</body>
</html>


