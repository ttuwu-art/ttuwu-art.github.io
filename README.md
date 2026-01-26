<html lang="es">
<head>
  <meta charset="UTF-8" />
  <title>ttuwu</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: #000;
      font-family: Arial, Helvetica, sans-serif;
      display: flex;
      justify-content: center;
    }

    .container {
      width: 100%;
      max-width: 900px;
      padding: 0 24px;
      text-align: center;
    }

    /* FADE IN */
    .fade {
      opacity: 0;
      animation: fadeIn 1.4s ease-out forwards;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(6px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    h1 {
      margin-top: 180px; /* espacio extra arriba */
      margin-bottom: 140px;
      font-size: 48px;
      font-weight: normal;
      color: #3a86ff;
    }

    iframe {
      border: none;
      outline: none;
      display: block;
      border-radius: 12px;
    }

    .block {
      max-width: 700px;
      margin: 0 auto 220px auto; /* separación grande */
    }

    .sc-caption {
      display: none; /* oculta texto extra de SoundCloud */
    }
  </style>
</head>

<body>
  <div class="container fade">

    <!-- SOUNDCLOUD NUEVO (ARRIBA DE TODO) -->
    <div class="block">
      <iframe
        width="100%"
        height="300"
        scrolling="no"
        allow="autoplay"
        src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/soundcloud%253Atracks%253A2254157330&auto_play=true&visual=true">
      </iframe>
    </div>

    <!-- SOUNDCLOUD ORIGINAL -->
    <div class="block">
      <iframe
        width="100%"
        height="166"
        scrolling="no"
        allow="autoplay"
        src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/soundcloud%253Atracks%253A2229331223&auto_play=true">
      </iframe>
    </div>

    <!-- SPOTIFY 1 -->
    <div class="block">
      <iframe
        src="https://open.spotify.com/embed/playlist/499zQTxAALSLh6x1tsryxn?utm_source=generator"
        width="100%"
        height="352"
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
        loading="lazy">
      </iframe>
    </div>

    <!-- SPOTIFY 2 -->
    <div class="block">
      <iframe
        src="https://open.spotify.com/embed/playlist/6xnl7nTO7iiw4xqfMluyMy?utm_source=generator"
        width="100%"
        height="352"
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
        loading="lazy">
      </iframe>
    </div>

  </div>
</body>
</html>
