Walmart
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Walmart</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>Walmart</h1>
    <nav>
      <ul>
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#productos">Productos</a></li>
      </ul>
    </nav>
  </header>

  <section id="inicio">
    <h2>Bienvenido a Walmart</h2>
    <p>Tu tienda online de confianza para productos de cocina y más.</p>
  </section>

  <section id="productos">
    <h2>Nuestros Productos</h2>
    <div class="producto">
      <img src="https://via.placeholder.com/200" alt="Sartenes">
      <h3>Paquete de Sartenes</h3>
      <p>Incluye 3 sartenes antiadherentes. Precio: $29.99</p>
      <button onclick="pagar('sartenes')">Comprar</button>
    </div>

    <div class="producto">
      <img src="https://via.placeholder.com/200" alt="Artículos chinos">
      <h3>Artículos Chinos</h3>
      <p>Variedad de productos decorativos y utilitarios. Precio: $15.99</p>
      <button onclick="pagar('articulos')">Comprar</button>
    </div>
  </section>

  <script src="script.js"></script>
</body>
</html>


body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #ffffff;
  color: #000;
}

header {
  background-color: #0071ce;
  color: white;
  padding: 1em;
  text-align: center;
}

nav ul {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
}

nav li {
  margin: 0 1em;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

section {
  padding: 2em;
  text-align: center;
}

.producto {
  border: 1px solid #ccc;
  border-radius: 10px;
  padding: 1em;
  margin: 1em auto;
  max-width: 300px;
}

.producto img {
  max-width: 100%;
  border-radius: 10px;
}

button {
  background-color: #0071ce;
  color: white;
  border: none;
  padding: 0.7em 1.2em;
  font-size: 1em;
  cursor: pointer;
  border-radius: 5px;
}

button:hover {
  background-color: #005fa3;
}

function pagar(producto) {
  let url = "";

  if (producto === 'sartenes') {
    url = "https://www.paypal.com/pay?product=sartenes";
  } else if (producto === 'articulos') {
    url = "https://www.paypal.com/pay?product=articulos";
  }

  window.open(url, '_blank');
}
