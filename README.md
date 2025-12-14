  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <style>
    /* RESET BÁSICO */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #000;
      color: #fff;
      font-family: Arial, Helvetica, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      min-height: 100vh;
    }

    /* CONTENIDO CON FADE IN */
    .fade {
      opacity: 0;
      animation: fadeIn 1.6s ease-out forwards;
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
      margin-top: 80px;
      margin-bottom: 60px;
      font-size: 48px;
      font-weight: normal;
      color: #2f6bff;
    }

    .soundcloud {
      width: 100%;
      max-width: 700px;
    }

    .spacer {
      height: 300px;
    }
  </style>
<body>

  <div class="soundcloud fade">
    <iframe
      width="100%"
      height="166"
      scrolling="no"
      frameborder="no"
      allow="autoplay"
      src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/soundcloud%253Atracks%253A2229331223&color=%23ff5500&auto_play=true&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true">
    </iframe>

    <div style="
      font-size: 10px;
      color: #cccccc;
      line-break: anywhere;
      word-break: normal;
      overflow: hidden;
      white-space: nowrap;
      text-overflow: ellipsis;
      font-family: Interstate, Lucida Grande, Lucida Sans Unicode, Lucida Sans, Garuda, Verdana, Tahoma, sans-serif;
      font-weight: 100;
    ">
      <a href="https://soundcloud.com/mauricio-rosas-hernandez" target="_blank" style="color:#cccccc; text-decoration:none;">
        Mauricio Rosas-Hernández
      </a>
      ·
      <a href="https://soundcloud.com/mauricio-rosas-hernandez/marcha-x-palestina00095900" target="_blank" style="color:#cccccc; text-decoration:none;">
        marcha x palestina00095900
      </a>
    </div>
  </div>

  <div class="spacer"></div>
</body>
