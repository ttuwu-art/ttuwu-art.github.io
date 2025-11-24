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
      color: #3a86ff; /* azul */
      font-family: Arial, sans-serif;
      overflow-x: hidden;
      padding-left: 10px; /* alineación izquierda */
    }

    h2 {
      text-align: left;
      margin-left: 0;
    }

    .container {
      width: 100%;
      display: flex;
      flex-direction: column;
      gap: 80px;
      padding: 50px 0;
    }

    .item {
      width: 100%;
      max-width: 800px;
      margin-left: 0;
    }

    model-viewer {
      width: 100%;
      height: 500px;
      background: #111;
      border-radius: 12px;
    }

    .contacto {
      margin-top: 80px;
      margin-bottom: 60px;
      text-align: left;
    }

    .btn {
      display: block;
      margin: 12px 0;
      padding: 14px 22px;
      width: 240px;
      text-align: left;
      border-radius: 8px;
      background: #2b2b2b;   /* gris */
      color: #3a86ff;        /* azul */
      text-decoration: none;
      border: 1px solid #555;
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
      <h2>Modelo 1 / モデル1</h2>
      <model-viewer src="modelo1.glb" camera-controls auto-rotate disable-zoom="false"></model-viewer>
    </div>

    <div class="item">
      <h2>Modelo 2 / モデル2</h2>
      <model-viewer src="modelo2.glb" camera-controls auto-rotate disable-zoom="false"></model-viewer>
    </div>

    <div class="item">
      <h2>Modelo 3 / モデル3</h2>
      <model-viewer src="modelo3.glb" camera-controls auto-rotate disable-zoom="false"></model-viewer>
    </div>

  </div>

  <div class="contacto">

    <h2>Contacto / 連絡先</h2>

    <a class="btn" href="https://wa.me/5215533677056" target="_blank">WhatsApp / ワッツアップ</a>
    <a class="btn" href="mailto:tucorreo@gmail.com" target="_blank">Correo / メール</a>
    <a class="btn" href="https://instagram.com/ttuwu_________________________" target="_blank">Instagram / インスタグラム</a>

  </div>

</body>
</html>
