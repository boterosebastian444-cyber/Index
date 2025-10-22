
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Z-Shoes</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #696464;
    }
    header {
      background-color: #A1301B;
      color: white;
      padding: 20px 0;
      text-align: center;
    }
    header img {
      width: 80px;
      height: auto;
      vertical-align: middle;
    }
    header h1 {
      display: inline-block;
      margin-left: 15px;
      font-size: 2.5rem;
      vertical-align: middle;
    }
    nav {
      text-align: center;
      background-color: #333;
      padding: 10px 0;
    }
    nav button {
      margin: 0 10px;
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      background-color: #A1301B;
      color: white;
      border: none;
      border-radius: 5px;
    }
    nav button:hover {
      background-color: #c84e34;
    }
    section {
      display: none;
      padding: 30px;
      background-color: white;
    }
    section.active {
      display: block;
    }
    .catalogo {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 20px;
      gap: 20px;
    }
    .producto {
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
      width: 250px;
      text-align: center;
      padding: 15px;
    }
    .producto img {
      width: 100%;
      height: auto;
      border-radius: 5px;
    }
    .producto h3 {
      margin: 10px 0 5px;
    }

    .producto p {
      margin: 0;
      color: #444;
    }
  </style>
</head>
<body>

  <header>
    <img src="https://cdn.leonardo.ai/users/0dc9f820-551d-4462-aa19-e68ef0e064ce/generations/80619bd4-756b-47be-b669-7cf1d12923c8/segments/2:4:1/Lucid_Origin_Crear_un_logo_minimalista_en_blanco_y_negro_que_s_1.jpg" alt="Logo Z-Shoes">
    <h1>Z-Shoes</h1>
  </header>

  <nav>
    <button onclick="mostrarSeccion('pagina1')">Página principal</button>
    <button onclick="mostrarSeccion('pagina2')">Juegos</button>
    <button onclick="mostrarSeccion('pagina3')">Registro</button>
  </nav>

  <!-- Página principal -->
  <section id="pagina1" class="active">
    <h2>Bienvenido a Z-Shoes</h2>
    <p>En <strong>Z-Shoes</strong> encontrarás la mejor selección de zapatos para cada ocasión. Comodidad, estilo y calidad al mejor precio.</p>

    <div class="catalogo">
      <div class="producto">
        <img src="https://cdn.leonardo.ai/users/0dc9f820-551d-4462-aa19-e68ef0e064ce/generations/e3c754ae-d70d-4d7e-8111-0c03435c03de/segments/4:4:1/Lucid_Origin_Disea_una_variedad_de_estilos_de_zapatos_deportiv_3.jpg" alt="Zapato 1">
        <h3>Zapato Deportivo Z-one</h3>
        <p>$59.999</p>
      </div>

      <div class="producto">
        <img src="https://cdn.leonardo.ai/users/0dc9f820-551d-4462-aa19-e68ef0e064ce/generations/e3c754ae-d70d-4d7e-8111-0c03435c03de/segments/1:4:1/Lucid_Origin_Disea_una_variedad_de_estilos_de_zapatos_deportiv_0.jpg" alt="Zapato 2">
        <h3>Zapato Casual Z-two</h3>
        <p>$45.999</p>
      </div>

      <div class="producto">
        <img src="https://cdn.leonardo.ai/users/0dc9f820-551d-4462-aa19-e68ef0e064ce/generations/b11c0a28-a3dc-4df1-b974-b39c5ab4792e/segments/1:4:1/Lucid_Origin_Disea_unos_zapatos_con_color_negro_y_blancos_que__0.jpg" alt="Zapato 3">
        <h3>Zapato Zamu-Z</h3>
        <p>$89.999</p>
      </div>

      <div class="producto">
        <img src="https://cdn.leonardo.ai/users/0dc9f820-551d-4462-aa19-e68ef0e064ce/generations/943ce33c-8a39-4cd5-9d69-f4a1c76b9597/segments/1:4:1/Lucid_Origin_Disea_unos_zapatos_innovadores_y_contemporneos_qu_0.jpg" alt="Zapato 4">
        <h3>Zapatos Style of Zamurai</h3>
        <p>$120.999</p>
      </div>
    </div>
  </section>
  <!-- Juegos -->
  <section id="pagina2">
    <h2>Juegos</h2>
    <p>Aquí podrás divertirte con nuestros minijuegos mientras exploras Z-Shoes.</p>
    <iframe src="https://www.retrogames.cc/embed/40615-super-mario-bros-nes.html" width="800" height="600" style="border:none;"></iframe>
  </section>
  <!-- Registro -->
  <section id="pagina3">
    <h2>Registro</h2>
    <form>
      <label for="usuario">Usuario:</label><br />
      <input type="text" id="usuario" name="usuario" required><br /><br />
      <label for="email">Correo electrónico:</label><br />
      <input type="email" id="email" name="email" required><br /><br />
      <label for="password">Contraseña:</label><br />
      <input type="password" id="password" name="password" required><br /><br />
      <button type="submit">Registrarse</button>
    </form>
  </section>
  <script>
    function mostrarSeccion(id) {
      const secciones = document.querySelectorAll('section');
      secciones.forEach(sec => sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>
</body>
</html>
