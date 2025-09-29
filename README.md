<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Siete Sopas - Página Oficial</title>
  <style>
    :root{--accent:#c0392b;--muted:#666;--card:#fff;--bg:#f5f5f5}
    *{box-sizing:border-box}
    body{font-family:Inter,system-ui,Segoe UI,Roboto,"Helvetica Neue",Arial; margin:0; background:var(--bg); color:#222}
    header{background:linear-gradient(90deg,#ffe5e0,#fff); padding:18px 16px; box-shadow:0 1px 6px rgba(0,0,0,.06);position:sticky;top:0;z-index:100}
    nav a{margin:0 10px;text-decoration:none;color:var(--accent);font-weight:600}
    .container{max-width:1000px;margin:18px auto;padding:0 16px}
    h1,h2,h3{color:var(--accent)}
    p.lead{margin:8px 0 0;color:var(--muted)}
    .card{background:var(--card);padding:14px;border-radius:12px;box-shadow:0 6px 18px rgba(0,0,0,.04);margin-bottom:16px}
    label{display:block;font-weight:600;margin-bottom:6px}
    input,select,textarea{width:100%;padding:10px;border:1px solid #e1e1e1;border-radius:8px}
    button{background:var(--accent);color:#fff;border:0;padding:10px 14px;border-radius:8px;cursor:pointer}
    img{max-width:100%;border-radius:12px;margin:8px 0}
    footer{margin:32px 0 60px;text-align:center;color:var(--muted)}

    /* Carrusel */
    .carousel{position:relative;overflow:hidden;border-radius:12px}
    .carousel img{width:100%;display:none}
    .carousel img.active{display:block}
    .carousel .controls{position:absolute;top:50%;left:0;right:0;display:flex;justify-content:space-between;transform:translateY(-50%);}
    .carousel button{background:rgba(0,0,0,0.5);border:0;color:#fff;padding:8px;cursor:pointer}

    iframe{border-radius:12px;border:0;width:100%;height:300px;margin-top:10px}
  </style>
</head>
<body>
  <header>
    <div class="container" style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap">
      <h1>Siete Sopas</h1>
      <nav>
        <a href="#inicio">Inicio</a>
        <a href="#menu">Menú</a>
        <a href="#reservas">Reservas</a>
        <a href="#pedidos">Pedidos</a>
        <a href="#nosotros">Nosotros</a>
        <a href="#ubicacion">Ubicación</a>
      </nav>
    </div>
  </header>

  <main>
    <!-- Página de inicio -->
    <section id="inicio" class="container">
      <div class="card">
        <h2>Bienvenidos a Siete Sopas</h2>
        <div class="carousel" id="carouselInicio">
          <img src="images/inicio1.jpg" alt="Interior de Siete Sopas" class="active" />
          <img src="images/menu.jpg" alt="Platos y sopas en Siete Sopas" />
          <img src="images/local.jpg" alt="Local de Siete Sopas" />
          <div class="controls">
            <button id="prev">❮</button>
            <button id="next">❯</button>
          </div>
        </div>
        <p class="lead">Cadena peruana nacida en Lima en 2016, famosa por sus sopas tradicionales disponibles las 24 horas.</p>
      </div>
    </section>

    <!-- Menú -->
    <section id="menu" class="container">
      <div class="card">
        <h2>Nuestro Menú</h2>
        <img src="images/menu.jpg" alt="Platos y sopas en Siete Sopas" />
        <ul>
          <li>Sopa Criolla - S/ 18.00</li>
          <li>Aguadito de Pollo - S/ 16.00</li>
          <li>Menestrón - S/ 14.00</li>
          <li>Patasca - S/ 20.00</li>
          <li>Sopa del día (pequeña) - S/ 10.00</li>
        </ul>
      </div>
    </section>

    <!-- Reservas -->
    <section id="reservas" class="container">
      <div class="card">
        <h2>Reservar mesa</h2>
        <img src="images/reservas.jpg" alt="Zona de reservas en Siete Sopas" />
        <form>
          <label>Nombre</label>
          <input placeholder="Tu nombre completo" />
          <label>Teléfono</label>
          <input placeholder="Ej: +51 9xx xxx xxx" />
          <label>Fecha</label>
          <input type="date" />
          <label>Hora</label>
          <input type="time" />
          <label>Personas</label>
          <select>
            <option>1</option><option>2</option><option>3</option><option>4</option><option>5</option><option>6+</option>
          </select>
          <button type="submit">Solicitar reserva</button>
        </form>
      </div>
    </section>

    <!-- Pedidos -->
    <section id="pedidos" class="container">
      <div class="card">
        <h2>Pedidos para llevar / Delivery</h2>
        <img src="images/pedidos.jpg" alt="Pedidos en Siete Sopas" />
        <form>
          <label>Dirección</label>
          <input placeholder="Calle, distrito, referencia" />
          <label>Método de pago</label>
          <select><option>Pago en local</option><option>Pago contra entrega</option><option>Transferencia</option></select>
          <button type="submit">Enviar pedido</button>
        </form>
      </div>
    </section>

    <!-- Nosotros -->
    <section id="nosotros" class="container">
      <div class="card">
        <h2>Sobre nosotros</h2>
        <img src="images/local.jpg" alt="Local de Siete Sopas" />
        <p class="lead">Siete Sopas nació en Lima en 2016 con la idea de ofrecer cada día siete sopas distintas, combinando tradición y sabor en un ambiente acogedor. Hoy en día es un punto de encuentro popular para familias, amigos y amantes de la comida peruana.</p>
      </div>
    </section>

    <!-- Ubicación -->
    <section id="ubicacion" class="container">
      <div class="card">
        <h2>Ubicación</h2>
        <p class="lead">Encuéntranos en Av. Arequipa 2394, Lince, Lima, Perú.</p>
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3900.9093100946097!2d-77.03652588518726!3d-12.074888891445448!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c8d7a733e7c3%3A0xe58d64df6e0e2f6a!2sSiete%20Sopas%20-%20Lince!5e0!3m2!1ses!2spe!4v1695933876204!5m2!1ses!2spe" allowfullscreen="" loading="lazy"></iframe>
      </div>
    </section>

    <footer>
      <p class="small">Prototipo en español — Reservas y pedidos en línea.</p>
    </footer>
  </main>

  <script>
    const images = document.querySelectorAll('#carouselInicio img');
    let current = 0;

    function showImage(index){
      images.forEach((img,i)=> img.classList.toggle('active', i===index));
    }

    document.getElementById('prev').addEventListener('click',()=>{
      current = (current-1+images.length)%images.length;
      showImage(current);
    });

    document.getElementById('next').addEventListener('click',()=>{
      current = (current+1)%images.length;
      showImage(current);
    });

    // Auto-play cada 4s
    setInterval(()=>{
      current = (current+1)%images.length;
      showImage(current);
    },4000);
  </script>
</body>
</html>
