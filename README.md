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
}

.product img {
  width:100%;
  height:200px;
  object-fit:cover;
}

.p-body {
  padding:10px;
  text-align:center;
}

.p-title { font-weight:bold; }
.price { margin:6px 0; font-weight:bold; }

.btn {
  display:inline-block;
  padding:8px 12px;
  background:#25D366;
  color:#fff;
  text-decoration:none;
  border-radius:5px;
}

footer {
  background:#111;
  color:#fff;
  text-align:center;
  padding:20px;
}

footer a {
  color:#ffcc00;
  text-decoration:none;
  font-weight:bold;
}
</style>

<script>
function comprar(producto) {
  const phone = "524428655081";
  const mensaje = encodeURIComponent(
    "Hola quiero comprar la gorra " + producto
  );

  if (/iPhone|iPad|iPod/i.test(navigator.userAgent)) {
    window.location.href =
      "whatsapp://send?phone=" + phone + "&text=" + mensaje;
  } else {
    window.open(
      "https://api.whatsapp.com/send?phone=" + phone + "&text=" + mensaje,
      "_blank"
    );
  }
}
</script>
</head>

<body>

<header>
  <h1>Junior Caps JR</h1>
  <p>Gorras estilo New Era calidad G5</p>
</header>

<section class="catalogo">

<article class="product">
<img src="https://i.imgur.com/HLlskRP.jpg">
<div class="p-body">
<div class="p-title">NY Classic – Negro</div>
<div class="price">$300 MXN</div>
<a class="btn" onclick="comprar('NY Classic Negro')">Comprar</a>
</div>
</article>

<article class="product">
<img src="https://imgur.com/FwFlSJC.jpg">
<div class="p-body">
<div class="p-title">31 NY black – Negro</div>
<div class="price">$2,000 MXN</div>
<a class="btn" onclick="comprar('31 NY black Negro')">Comprar</a>
</div>
</article>

<article class="product">
<img src="https://imgur.com/dDoFbWn.jpg">
<div class="p-body">
<div class="p-title">Barbas Galaxy – Negro</div>
<div class="price">$2,000 MXN</div>
<a class="btn" onclick="comprar('Barbas Galaxy Negro')">Comprar</a>
</div>
</article>

<article class="product">
<img src="https://imgur.com/2WIk8sw.jpg">
<div class="p-body">
<div class="p-title">LA clauds 31 – Negro</div>
<div class="price">$2,000 MXN</div>
<a class="btn" onclick="comprar('LA clauds 31 Negro')">Comprar</a>
</div>
</article>

<article class="product">
<img src="https://imgur.com/ygpFh1E.jpg">
<div class="p-body">
<div class="p-title">$ad boy DH – Negro</div>
<div class="price">$1,500 MXN</div>
<a class="btn" onclick="comprar('ad boy DH Negro')">Comprar</a>
</div>
</article>

<article class="product">
<img src="https://imgur.com/LOTRkoR.jpg">
<div class="p-body">
<div class="p-title">Rocstar CT – Negro</div>
<div class="price">$1,600 MXN</div>
<a class="btn" onclick="comprar('Rocstar CT Negro')">Comprar</a>
</div>
</article>

<article class="product">
<img src="https://imgur.com/hKV7oZN.jpg">
<div class="p-body">
<div class="p-title">Chorme CT – Negro</div>
<div class="price">$1,600 MXN</div>
<a class="btn" onclick="comprar('Chorme CT Negro')">Comprar</a>
</div>
</article>

</section>

<footer>
  <p>Síguenos en Instagram:</p>
  <a href="https://www.instagram.com/junior_hats_jr" target="_blank">
    @junior_hats_jr
  </a>
</footer>

</body>
</html>


