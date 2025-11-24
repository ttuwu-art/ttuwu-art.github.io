<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>ttuwu — 3D Gallery</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@200;400;600&display=swap" rel="stylesheet" />

<style>
    body {
        background:#000;
        color:#4aa3ff;
        font-family:'Inter', sans-serif;
        margin:0;
        padding:20px;
    }

    h1 { margin-bottom:10px; }

    /* ----- GALLERY ----- */
    .gallery {
        display:flex;
        flex-direction:column;
        gap:40px;
        margin-top:20px;
    }

    model-viewer {
        width: 300px;
        height: 300px;
        background:#000;
    }

    /* ----- HAMBURGER MENU ----- */
    .menu-btn {
        width:35px;
        cursor:pointer;
        margin-bottom:20px;
    }

    .bar {
        height:4px;
        background:#4aa3ff;
        margin:6px 0;
        width:100%;
        transition:.3s;
    }

    /* ----- SIDE MENU ----- */
    #sideMenu {
        position:fixed;
        top:0;
        left:-250px;
        width:250px;
        height:100%;
        background:#000;
        border-right:1px solid #4aa3ff;
        padding:40px 20px;
        transition:0.3s ease;
    }

    #sideMenu a {
        display:block;
        color:#4aa3ff;
        text-decoration:none;
        margin:15px 0;
        font-size:18px;
    }

    #sideMenu.open {
        left:0;
    }
</style>

<script>
function toggleMenu() {
    document.getElementById("sideMenu").classList.toggle("open");
}
</script>

<!-- Model Viewer -->
<script type="module" src="https://cdn.jsdelivr.net/npm/@google/model-viewer/dist/model-viewer.min.js"></script>
</head>

<body>

<!-- MENU BUTTON -->
<div class="menu-btn" onclick="toggleMenu()">
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
</div>

<!-- SIDE MENU -->
<div id="sideMenu">
    <a href="imagen.html">Imagen / 画像</a>
    <a href="sonido.html">Sonido / 音</a>
    <a href="video.html">Video / ビデオ</a>
    <a href="procesos.html">Procesos / プロセス</a>
</div>

<h1>Galería 3D / 3Dギャラリー</h1>

<div class="gallery">
    <model-viewer src="models/model1.glb" auto-rotate camera-controls></model-viewer>
    <model-viewer src="models/model2.glb" auto-rotate camera-controls></model-viewer>
    <model-viewer src="models/model3.glb" auto-rotate camera-controls></model-viewer>
</div>

</body>
</html>
