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
