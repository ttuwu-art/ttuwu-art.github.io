# ttuwu-art.github.io
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Galería 3D – Mauricio</title>

  <!-- Model Viewer -->
  <script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>

  <style>
    body {
      margin: 0;
      background: #000;
      color: #fff;
      font-family: Arial, sans-serif;
      overflow-x: hidden;
    }

    .container {
      width: 100%;
      display: flex;
      flex-direction: column;
      gap: 100px;
      padding: 40px 0;
    }

    .item {
      width: 100%;
      max-width: 800px;
      margin: auto;
      text-align: center;
    }

    model-viewer {
      width: 100%;
      height: 500px;
      background: #111;
      border-radius: 12px;
    }

    .contacto {
      text-align: center;
      margin-top: 80px;
      margin-bottom: 60px;
    }

    .btn {
      display: block;
      margin: 10px auto;
      padding: 14px 22px;
      width: 220px;
      text-align: center;
      border-radius: 8px;
      background: #222;
      color: #fff;
      text-decoration: none;
      border: 1px solid #444;
      font-size: 16px;
      transition: 0.2s;
    }

    .btn:hover {
      background: #444;
    }
  </style>
</head>

<body>

  <div class="container">

    <div class="item">
      <h2>Modelo 1</h2>
      <model-viewer src="modelo1.glb" camera-controls auto-rotate disable-zoom="false"></model-viewer>
    </div>

    <div class="item">
      <h2>Modelo 2</h2>
      <model-viewer src="modelo2.glb" camera-controls auto-rotate disable-zoom="false"></model-viewer>
    </div>

    <div class="item">
      <h2>Modelo 3</h2>
      <model-viewer src="modelo3.glb" camera-controls auto-rotate disable-zoom="false"></model-viewer>
    </div>

  </div>

  <div class="contacto">
    <h2>Contacto</h2>

    <a class="btn" href="https://wa.me/521XXXXXXXXXX" target="_blank">WhatsApp</a>
    <a class="btn" href="mailto:tucorreo@gmail.com" target="_blank">Correo</a>
    <a class="btn" href="https://instagram.com/TUUSUARIO" target="_blank">Instagram</a>
    <a class="btn" href="https://linktr.ee/TUUSUARIO" target="_blank">Otras redes</a>
