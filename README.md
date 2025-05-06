<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ni una más</title>
  <style>
    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background-color: #f5e8f6;
      color: #2e2b4f;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px;
    }

    header {
      background-color: #fff;
      padding: 20px;
      text-align: center;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    header nav a {
      margin: 0 15px;
      font-weight: bold;
    }

    .hero,
    .section {
      display: flex;
      align-items: center;
      background-color: #fff;
      padding: 40px;
      margin: 20px 0;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      flex-wrap: wrap;
    }

    .hero img,
    .section img {
      width: 300px;
      margin-right: 40px;
      max-width: 100%;
      height: auto;
      border-radius: 10px;
    }

    .hero-text,
    .section-text {
      flex: 1;
      min-width: 250px;
    }

    .hero h1,
    .section-title {
      font-size: 2.5em;
      margin-bottom: 20px;
      color: #4a148c;
    }

    .buttons {
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
    }

    .buttons button {
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      font-size: 1em;
      cursor: pointer;
    }

    .btn-red {
      background-color: #e0324c;
      color: white;
    }

    .btn-light {
      background-color: #dfc7f6;
      color: #2e2b4f;
    }

    .violence-types {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
      gap: 20px;
      margin-top: 20px;
    }

    .violence-types a div {
      background-color: #e8d9f5;
      padding: 20px;
      border-radius: 10px;
      text-align: center;
      flex: 1;
      min-width: 150px;
      font-weight: bold;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    .help a button {
      background-color: #4a148c;
      color: white;
      padding: 15px 30px;
      border: none;
      border-radius: 10px;
      font-size: 1em;
      cursor: pointer;
    }

    #btn-arriba {
      position: fixed;
      bottom: 25px;
      right: 25px;
      background-color: #e0324c;
      color: white;
      border: none;
      border-radius: 50%;
      width: 50px;
      height: 50px;
      font-size: 24px;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
      display: none;
      z-index: 1000;
    }
  </style>
</head>
<body>

  <header>
    <nav>
      <a href="#inicio">Inicio</a>
      <a href="#tipos">Tipos de violencia</a>
      <a href="#ayuda">¿PUEDES RESPONDER?</a>
    </nav>
  </header>

  <div class="container">

    <!-- HERO / INICIO -->
    <section class="hero" id="inicio">
      <img src="https://i.pinimg.com/736x/ea/7d/d2/ea7dd2e1dafc2278eca6ddca759346fe.jpg" alt="Mujer con señal de alto">
      <div class="hero-text">
        <h1>Ni una más. Todas merecemos vivir libres y seguras.</h1>
        <div class="buttons">
          <a href="https://espanol.thehotline.org/" target="_blank">
            <button class="btn-red">Pide ayuda ahora</button>
          </a>
        </div>
      </div>
    </section>

 
    <!-- TIPOS DE VIOLENCIA -->
    <section class="section" id="tipos">
      <div class="section-text">
        <h2 class="section-title">Tipos de violencia</h2>
        <p>Existen distintos tipos de violencia que pueden afectar a las mujeres. Conocerlos es el primer paso para identificarlos y denunciarlos.</p>
        <div class="violence-types">
          <a href="violencia-fisica.html" target="_blank"><div>Física</div></a>
          <a href="violencia-psicologica.html" target="_blank"><div>Psicológica</div></a>
          <a href="violencia-sexual.html" target="_blank"><div>Sexual</div></a>
          <a href="violencia-economica.html" target="_blank"><div>Económica</div></a>
          <a href="violencia-digital.html" target="_blank"><div>Digital</div></a>
        </div>
      </div>
    </section>

    <!-- ¿PUEDES RESPONDER? -->
    <section class="section" id="ayuda">
      <div class="section-text">
        <h2 class="section-title">¿PUEDES RESPONDER?</h2>
        <p>Si estás en una situación de riesgo, hay organizaciones que pueden ayudarte. Busca apoyo profesional y recursos disponibles en tu comunidad.</p>
        <div class="help">
          <a href="recursos.html" target="_blank"><button>FORMULARIO</button></a>
        </div>
      </div>
    </section>

  </div>

<!-- ... (tu código anterior se mantiene igual) -->

  <!-- BOTÓN DE IR ARRIBA -->
  <button id="btn-arriba" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">↑</button>

  <script>
    const btnArriba = document.getElementById("btn-arriba");
    window.addEventListener("scroll", () => {
      btnArriba.style.display = window.scrollY > 300 ? "block" : "none";
    });
  </script>

<footer style="background-color: #4a148c; color: #fff; padding: 20px; text-align: center;">
  <p>&copy; 2025 Conciencia Contra la Violencia. Todos los derechos reservados.</p>
  <p>Desarrollado por: ROSALBA, JALIL CALVO, SERGIO IVAN, ANUAR TOBIAS</p>
  <p>Contacto: 
    <a href="mailto:info@concienciaviolencia.org" style="color: #ddd;">info@concienciaviolencia.org</a>
  </p>
  <p>
    <a href="/aviso-legal.html" style="color: #ddd; margin: 0 10px;">Aviso legal</a> |
    <a href="/politica-privacidad.html" style="color: #ddd; margin: 0 10px;">Política de privacidad</a> |
    <a href="/recursos.html" style="color: #ddd; margin: 0 10px;">Recursos de ayuda</a>
  </p>
</footer>

  </footer>

</body>
</html>

</body>
</html>
