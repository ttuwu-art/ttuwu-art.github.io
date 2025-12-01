<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing Page Básica</title>

    <style>
        body {
            margin: 0;
            background-color: #000; /* Fondo negro */
            font-family: Arial, sans-serif;
            color: white;
            text-align: center;
        }

        h1 {
            margin-top: 40px;
            font-size: 28px;
            letter-spacing: 1px;
        }

        .gallery {
            margin-top: 50px;
        }

        .gallery img {
            width: 80%;
            max-width: 600px;
            border-radius: 6px;
            border: 1px solid #444;
        }

        /* Espacio extra abajo */
        .spacer {
            height: 300px;
        }
    </style>
</head>

<body>

    <h1>Mi Landing Page</h1>

    <div class="gallery">
        <!-- Cambia "imagen.jpg" por el nombre REAL del archivo que subas -->
        <img src="imagen.jpg" alt="Mi imagen">
    </div>

    <div class="spacer"></div>
</body>
</html>
