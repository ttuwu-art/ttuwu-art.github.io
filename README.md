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

    /* FADE IN SUAVE */
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
      margin-top: 140px;
      margin-bottom: 120px;
      font-size: 48px;
      font-weight: normal;
      color: #3b6cff;
    }

    .soundcloud,
    .spotify {
      max-width: 700px;
      margin-left: auto;
      margin-right: auto;
    }

    .soundcloud {
      margin-bottom: 160px; /* separación clara */
    }

    iframe {
      border: none;
      outline: none;
      display: block;
    }

    .spacer {
      height: 320px;
    }
  </style>
</head>

<body>
  <div class="container fade">

    <!-- SOUNDCLOUD -->
    <div class="soundcloud">
      <iframe
        width="100%"
        height="166"
        scrolling="no"
        allow="autoplay"
        src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/soundcloud%253Atracks%253A2229331223&auto_play=true">
      </iframe>
    </div>

    <!-- SPOTIFY -->
    <div class="spotify">
      <iframe
        src="https://open.spotify.com/embed/playlist/6xnl7nTO7iiw4xqfMluyMy"
        width="100%"
        height="352"
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
        loading="lazy">
      </iframe>
    </div>

    <div class="spacer"></div>

  </div>
</body>
</html>


    <div class="spacer"></div>

  </div>
</body>
</html>
