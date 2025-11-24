<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>ttuwu</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&display=swap" rel="stylesheet" />

<style>
    body {
        background:#000;
        color:#fff;
        font-family:'Inter', sans-serif;
        margin:0;
    }

    /* Contenedor general */
    .container {
        width: 65%;
        margin: 0 auto;
        padding-top: 40px;
    }

    /* Viewer */
    .viewer {
        background:#000;
        border:1px solid #333;
        height:300px;
        margin-bottom:20px;
    }

    /* MENÚ HAMBURGUESA */
    .hamburger {
        position: fixed;
        top: 20px;
        right: 20px;
        width: 30px;
        cursor: pointer;
        z-index: 1000;
    }
    .hamburger div {
        height: 4px;
        background: #fff;
        margin: 6px 0;
        border-radius: 4px;
    }

    .menu {
        position: fixed;
        top: 0;
        right: -200px;
        width:200px;
        height:100%;
        background:#111;
        padding:40px 20px;
        transition:0.3s;
    }

    .menu.open {
        right: 0;
    }

    .menu a {
        display: block;
        color:#4ab3ff;
        font-size:20px;
        margin-bottom:20px;
        text-decoration:none;
    }
</style>

<script>
function toggleMenu() {
    document.getElementById("menu").classList.toggle("open");
}
</script>
</head>

<body>

<!-- Hamburguesa -->
<div class="hamburger" onclick="toggleMenu()">
    <div></div><div></div><div></div>
</div>

<!-- Menú -->
<div id="menu" class="menu">
    <a href="imagen.html">Imagen</a>
    <a href="sonido.html">Sonido</a>
    <a href="video.html">Video</a>
    <a href="procesos.html">Procesos</a>
</div>

<div class="container">

    <h1>Modelos</h1>

    <div class="viewer"></div>

    <p>Aquí irán tus modelos 3D, imágenes o renders.</p>

</div>

</body>
</html>
