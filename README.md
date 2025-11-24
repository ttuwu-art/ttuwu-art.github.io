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
      padding-left: 10px; /* alineado a la izquierda */
    }

    h2 {
      margin: 0 0 12px 0;
      font-weight: normal;
    }

    .container {
      width: 100%;
      display: flex;
      flex-direction: column;
      gap: 60px;
      padding: 40px 0;
    }

    .item {
      width: 100%;
      max-width: 700px;
    }

    model-viewer {
      width: 100%;
      height: 330px; /* 🔥 un tercio más pequeño */
      background: #000 !important; /* 🔥 negro puro */
      border-radius: 10px;
    }

    .contacto {
      margin-top: 60px;
      margin-bottom: 80px;
    }

    .btn {
      display: block;
      margin: 12px 0;
      padding: 14px 20px;
      width: 240px;
      text-align: left;
      border-radius: 8px;
      background: #333;   /* gris */
      color: #3a86ff;     /* azul */
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
      <model-viewer src="modelo1.glb" camera-controls auto-rotate></model-viewer>
    </div>

    <div class="item">
      <h2>Modelo 2 / モデル2</h2>
      <model-viewer src="modelo2.glb" camera-controls auto-rotate></model-viewer>
    </div>

    <div class="item">
      <h2>Modelo 3 / モデル3</h2>
      <model-viewer src="modelo3.glb" camera-controls auto-rotate></model-viewer>
    </div>

  </div>

  <div class="contacto">
    <h2>Contacto / 連絡先</h2>

    <a class="btn" href="https://wa.me/5215533677056" target="_blank">WhatsApp / ワッツアップ</a>
    <a class="btn" href="mailto:tucorreo@gmail.com" target="_blank">Correo / メール</a>
    <a class="btn" href="https://instagram.com/ttuwu_________________________" target="_blank">
      Instagram / インスタグラム
    </a>
  </div>

</body>
</html>
