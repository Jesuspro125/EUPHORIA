<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Clan EUPHORIA - Free Fire</title>
  <style>
    :root {
      --bg-color: #e0f7fa;
      --accent-color: #0288d1;
      --text-color: #333;
      --box-bg: #ffffff;
      --main-bg: #d7f4f9;
      
      footer {
  background-color: #d3d3d3; /* gris claro */
  text-align: center;
  padding: 1rem;
  font-size: 0.9rem;
  color: #333;
}

footer a {
  color: #0288d1; /* el azul de tu tema boys */
  text-decoration: underline;
}
      
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--bg-color);
      color: var(--text-color);
      transition: background-color 0.5s, color 0.5s;
    }

    header {
      background-color: var(--accent-color);
      padding: 2rem 1rem;
      text-align: center;
      border-radius: 20px;
      margin: 20px auto;
      width: fit-content;
      max-width: 90%;
      color: white;
      font-size: 2rem;
      font-weight: bold;
      box-shadow: 0 6px 12px rgba(0,0,0,0.1);
    }

    main {
      max-width: 900px;
      margin: auto;
      padding: 1.5rem;
      background-color: var(--main-bg);
      border-radius: 16px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      transition: background-color 0.5s;
    }

    .bienvenida {
      border: 2px dashed var(--accent-color);
      padding: 1.5rem;
      border-radius: 15px;
      background-color: var(--box-bg);
      margin-bottom: 2rem;
      transition: background-color 0.5s;
    }
    
    .mensaje-invitacion {
  margin: 1.5rem 0;
  padding: 1rem;
  border-left: 5px solid var(--accent-color);
  background-color: var(--box-bg);
  color: var(--text-color);
  border-radius: 10px;
  font-size: 1.05rem;
  transition: background-color 0.5s, color 0.5s;
}

    h2 {
      color: var(--accent-color);
      margin-top: 2rem;
    }

    p {
      font-size: 1.1rem;
      margin: 1rem 0;
    }

    .btn-action {
      padding: 0.8rem 1.5rem;
      margin: 1rem;
      font-size: 1rem;
      border: none;
      border-radius: 8px;
      background-color: var(--accent-color);
      color: white;
      cursor: pointer;
      transition: background-color 0.3s;
    }

    .btn-action:hover {
      background-color: #026aa7;
    }

    .theme-toggle {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: white;
      border: 2px solid var(--accent-color);
      border-radius: 50%;
      width: 55px;
      height: 55px;
      font-weight: bold;
      cursor: pointer;
      color: var(--accent-color);
      font-size: 0.8rem;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    #requisitos {
      display: none;
      margin-top: 1rem;
      text-align: left;
      padding: 1rem;
      border-radius: 10px;
      background-color: var(--box-bg);
      border: 2px solid var(--accent-color);
      transition: background-color 0.5s, border-color 0.5s;
    }

    #requisitos ul {
      padding-left: 1.5rem;
    }

    #requisitos li {
      margin-bottom: 0.7rem;
      font-size: 1.05rem;
    }

    .testimonios blockquote {
      background: #fff3cd;
      border-left: 6px solid #ffecb5;
      margin: 1rem 0;
      padding: 1rem;
      border-radius: 10px;
      font-style: italic;
    }

    .contacto a {
      display: inline-block;
      margin: 0.5rem;
      padding: 0.6rem 1rem;
      background-color: var(--accent-color);
      color: white;
      text-decoration: none;
      border-radius: 8px;
      transition: 0.3s;
    }

    .contacto a:hover {
      background-color: #026aa7;
    }

    .galeria {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
    }

    .galeria img {
      width: 100%;
      max-width: 180px;
      border-radius: 10px;
    }

    .carrusel {
      position: relative;
      overflow: hidden;
      width: 100%;
      max-width: 700px;
      margin: auto;
      border-radius: 12px;
      margin-top: 2rem;
    }

    .carrusel img {
      width: 100%;
      height: auto;
      display: none;
    }

    .carrusel img.active {
      display: block;
    }

    .carrusel-control {
      display: block;
      margin: 1rem auto;
      padding: 0.5rem 1rem;
      background-color: var(--accent-color);
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    @media (max-width: 600px) {
      .btn-action, .contacto a {
        width: 90%;
      }

      .galeria img {
        max-width: 100%;
      }

      .theme-toggle {
        width: 50px;
        height: 50px;
        font-size: 0.7rem;
      }
    }
  </style>
</head>
<body>
  <header>💥 Clan EUPHORIA 💥</header>
  
  
  <main>
    <div class="bienvenida">
      <h2>🎉 ¡Bienvenidos al Clan EUPHORIA!</h2>
      <h4> en la esquina inferior derecha encontrarás un botón flotante redondo para cambiar de tema según tu género</h4>
      <p>Somos una comunidad de jugadores apasionados por <strong>Free Fire</strong>. </p>
    </div>

    <button class="btn-action" onclick="mostrarMensajeInvitacion()">Quiero Unirme al Clan</button>
    <button class="btn-action" onclick="toggleRequisitos()">Ver Requisitos</button>

<div id="mensaje-invitacion" style="display: none;" class="mensaje-invitacion">
  📩 Mándanos un WhatsApp usando el botón al final de esta página en la sección de contacto para que recibas la ficha a llenar y poder proceder con tu incorporación.
</div>

<div id="requisitos">
  <h2>📋 Requisitos para Unirte</h2>
  <ul>
    <li>🆙🎮 Cuentas <strong> nivel 50 </strong>en adelante</li>
    <li>🔄📝 Cambio de <strong>nombre</strong> obligatorio</li>
    <li>💎🇲🇽🇧🇷 Cuentas <strong>diamante I</strong> en adelante en decla y br</li>
    <li>🔞 +16</li>
    <li>🏅💯 Cumplir con <strong>2,500</strong> de honor</li>
    <li>⚔️🕐 Guerra de clanes <strong>140-100</strong> min</li>
    <li>🧠🎯 Experiencia en <strong>vs 12vs12, compes, infinitos</strong></li>
    <li>📱💬🔥 Ser <strong>activos</strong> en vs y en grupos de ws</li>
    <li>🎉🤝👥 Participar de las <strong>dinámicas</strong> del clan</li>
  </ul>
</div>

    <h2>🌟 ¿Por qué unirte a EUPHORIA?</h2>
    <p>🏅 Nivel 7<br>🔥 Torneos semanales<br>🎯 Entrenamiento con los mejores<br>🏆 Premios exclusivos<br>🤝 Comunidad activa<br>💯  Activo<br>🌎  Top Global con Titulo<br>🏹  VS con Otros Clanes</p>
    
    <h2>💬 nuestro compromiso </h2>
    <div class="testimonios">
      <blockquote>"Al Entrar a EUPHORIA, Mejoras tu perfil y compromiso con el juego."</blockquote>
      <blockquote>"Al Entrar a EUPHORIA, Encontrarás grandes amigos para pasar el tiempo."</blockquote>
      <blockquote>"La mejor decisión que pudiste tomar es entrar, ¡Te va a encanta la comunidad!"</blockquote>
    </div>

    <h2>📸 Galería</h2>
    <div class="galeria">
      <img src="https://files.catbox.moe/n0lu6g.jpg" alt="img1">
      <h3>Imagen del clan EUPHORIA</h3>
      <img src="https://files.catbox.moe/na2ps3.jpg" alt="img2">
      <h3>Nivel del clan EUPHORIA</h3>
      <img src="https://files.catbox.moe/fluv1q.jpg" alt="img3">
      <h3>Título de gloria en top global</h3>
      <img src="https://files.catbox.moe/25hx3e.jpg" alt="img4">
      <h3>Emote exclusivo de nivel </h3>
    </div>
    
    <h2>🌟 ¿Por qué EUPHORIA es mejor que otros clanes?</h2>
    <p ⚫ Integrantes destacados<br> ⚫ Su nivel al máximo<br>⚫ Titulo de Guerra de clanes con top global<br>⚫ Racha de Victorias en VS<br>⚫ Viral en TikTok</p>
   

    <h2>🎞️ Carrusel de BOOYAHS en VS</h2>
    <div class="carrusel" id="carrusel">
      <img src="https://files.catbox.moe/a8qlfq.jpg" class="active" />
      <img src="https://files.catbox.moe/cikrq7.jpg" />
      <img src="https://files.catbox.moe/901b8y.jpg" />
      <img src="https://files.catbox.moe/0ar6de.jpg" />
      <img src="https://files.catbox.moe/a2tofr.jpg" />
    </div>
    <button class="carrusel-control" onclick="toggleCarrusel()">
      ⏸️ Pausar
    </button>

    <h2>📲 Contacto</h2>
    <div class="contacto">
      <a href="https://tiktok.com/@myeuphoria.ff" target="_blank">🎵 TikTok</a>
      <a href="https://www.instagram.com/myeuphoria.ff?igsh=aTA2azZxaDBldjdv" target="_blank">📸 Instagram</a>
      <a href="https://api.whatsapp.com/send?phone=+523350079670" target="_blank">💬 WhatsApp</a>
    </div>
  </main>

  <button class="theme-toggle" onclick="toggleTheme()">Modo<br>Boys</button>
  
<footer>
  <p>© 2025 José Zambrano.<a href="https://api.whatsapp.com/send?phone=+523350079670" target="_blank" style="color: black; text-decoration: underline;">
  Aviso Legal
</a>
</footer>
  
  <script>
    let currentTheme = 'boys';
window.addEventListener('DOMContentLoaded', () => {
  toggleTheme(); // Cambia a girls automáticamente
});
    let requisitosVisible = false;
    let carruselIndex = 0;
    let carruselPaused = false;

    const images = document.querySelectorAll("#carrusel img");

    function toggleTheme() {
      const root = document.documentElement;
      const toggleBtn = document.querySelector('.theme-toggle');

      if (currentTheme === 'boys') {
        // Cambiar a modo Girls
        root.style.setProperty('--bg-color', '#fce4ec');
        root.style.setProperty('--accent-color', '#ec407a');
        root.style.setProperty('--box-bg', '#fdeff4');
        root.style.setProperty('--main-bg', '#fddae6');
        toggleBtn.innerHTML = 'Modo<br>Girls';
        currentTheme = 'girls';
      } else {
        // Cambiar a modo Boys
        root.style.setProperty('--bg-color', '#e0f7fa');
        root.style.setProperty('--accent-color', '#0288d1');
        root.style.setProperty('--box-bg', '#ffffff');
        root.style.setProperty('--main-bg', '#d7f4f9');
        toggleBtn.innerHTML = 'Modo<br>Boys';
        currentTheme = 'boys';
      }
    }

    function toggleRequisitos() {
      const caja = document.getElementById('requisitos');
      requisitosVisible = !requisitosVisible;
      caja.style.display = requisitosVisible ? 'block' : 'none';
    }

    function showCarruselImage(index) {
      images.forEach((img, i) => {
        img.classList.toggle("active", i === index);
      });
    }

    function nextCarruselImage() {
      if (!carruselPaused) {
        carruselIndex = (carruselIndex + 1) % images.length;
        showCarruselImage(carruselIndex);
      }
    }

    setInterval(nextCarruselImage, 3000);

    function toggleCarrusel() {
      carruselPaused = !carruselPaused;
      document.querySelector(".carrusel-control").textContent = carruselPaused ? "▶️ Reanudar" : "⏸️ Pausar";
    }
    
    let mensajeVisible = false;

function mostrarMensajeInvitacion() {
  const mensaje = document.getElementById('mensaje-invitacion');
  mensajeVisible = !mensajeVisible;
  mensaje.style.display = mensajeVisible ? 'block' : 'none';
}

  </script>
</body>
</html>
