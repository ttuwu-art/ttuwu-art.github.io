<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ttuwu — Portfolio</title>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&display=swap" rel="stylesheet" />

  <!-- Model Viewer -->
  <script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>

  <style>
    body {
      margin: 0;
      padding: 0;
      background: #000;
      color: #4aa3ff;
      font-family: 'Inter', sans-serif;
      padding-left: 10px;
    }

    h1 {
      font-size: 22px;
      font-weight: 600;
      color: #4aa3ff;
      margin-top: 20px;
    }

    .viewer-container {
      width: 65%; /* 1/3 más pequeño */
      height: 300px;
      margin: 20px 0;
    }

    model-viewer {
      width: 100%;
      height: 100%;
      background-color: #000 !important;
    }

    .contact {
      margin-top: 20px;
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .btn {
      background: #444;
      color: #4aa3ff;
      padding: 10px 14px;
      border-radius: 6px;
      width: fit-content;
      text-decoration: none;
      font-size: 14px;
    }

    /* ---- NAV ---- */
    .menu-btn {
      position: fixed;
      top: 15px;
      right: 20px;
      width: 32px;
      height: 24px;
      cursor: pointer;
      z-index: 999;
    }

    .menu-btn div {
      width: 100%;
      height: 4px;
      background: #4aa3ff;
      margin: 4px 0;
      transition: 0.3s;
    }

    /* Menu panel */
    .menu-panel {
      position: fixed;
      top: 0;
      right: -250px;
      width: 250px;
      height: 100vh;
      background: #111;
      padding: 40px 20px;
      transition: 0.3s ease;
      display: flex;
      flex-direction: column;
      gap: 18px;
      z-index: 998;
    }

    .menu-panel a {
      color: #4aa3ff;
      font-size: 18px;
      text-decoration: none;
    }

    .menu-open .menu-panel {
      right: 0;
    }

    .menu-open .menu-btn div:nth-child(1) {
      transform: rotate(45deg) translate(6px, 6px);
    }

    .menu-open .menu-btn div:nth-child(2) {
      opacity: 0;
    }

    .menu-open .menu-btn div:nth-child(3) {
      transform: rotate(-45deg) translate(6px, -6px);
    }
  </style>
</head>
<body>

  <!-- MENU BUTTON -->
  <div class="menu-btn" id="menuBtn">
    <div></div>
    <div></div>
    <div></div>
  </div>

  <!-- MENU PANEL -->
  <nav class="menu-panel" id="menuPanel">
    <a href="#imagen">Imagen / 画像</a>
    <a href="#sonido">Sonido / 音</a>
    <a href="#video">Video / 映像</a>
    <a href="#procesos">Procesos / プロセス</a>
  </nav>

  <h1>ttuwu — Portfolio</h1>

  <!-- MODEL 1 -->
  <section id="imagen">
    <h2>Imagen / 画像</h2>
    <div class="viewer-container">
      <model-viewer src="model1.glb" auto-rotate camera-controls></model-viewer>
    </div>
  </section>

  <!-- MODEL 2 -->
  <section id="sonido">
    <h2>Sonido / 音</h2>
    <div class="viewer-container">
      <model-viewer src="model2.glb" auto-rotate camera-controls></model-viewer>
    </div>
  </section>

  <!-- MODEL 3 -->
  <section id="video">
    <h2>Video / 映像</h2>
    <div class="viewer-container">
      <model-viewer src="model3.glb" auto-rotate camera-controls></model-viewer>
    </div>
  </section>

  <section id="procesos">
    <h2>Procesos / プロセス</h2>
    <p>Documentación de procesos creativos, pruebas, bocetos y exploraciones.</p>
  </section>

  <div class="contact">
    <a class="btn" href="https://instagram.com/ttuwu_________________________">Instagram / インスタ</a>
    <a class="btn" href="https://wa.me/525533677056">WhatsApp / ワッツアップ</a>
    <a class="btn" href="mailto:correo@example.com">Correo / メール</a>
  </div>

  <script>
    const btn = document.getElementById("menuBtn");
    document.addEventListener("click", (e) => {
      if (btn.contains(e.target)) {
        document.body.classList.toggle("menu-open");
      } else {
        document.body.classList.remove("menu-open");
      }
    });
  </script>

</body>
</html>
