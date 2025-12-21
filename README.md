<a class="btn" href="#"
onclick="openWhatsApp('Hola quiero comprar la gorra NY Classic')">
Comprar
</a>

<script>
function openWhatsApp(msg) {
  const phone = '524428655081';
  const text = encodeURIComponent(msg);

  if (/iPhone|iPad|iPod/i.test(navigator.userAgent)) {
    window.location.href = `whatsapp://send?phone=${phone}&text=${text}`;
  } else {
    window.open(`https://api.whatsapp.com/send?phone=${phone}&text=${text}`, '_blank');
  }
}
</script>


