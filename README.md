<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Perfil Personal</title>
  <style>
    :root{
      --bg: #f7f9fc;
      --card: #ffffff;
      --accent: #2563eb;
      --muted: #556078;
      --radius: 12px;
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }

    html,body{height:100%;margin:0;background:var(--bg);color:#0f172a}
    .wrap{
      max-width:900px;
      margin:48px auto;
      padding:24px;
    }

    .card{
      background:var(--card);
      border-radius:var(--radius);
      box-shadow:0 6px 18px rgba(15,23,42,0.06);
      padding:20px;
    }

    .profile{
      display:flex;
      gap:20px;
      align-items:flex-start;
    }

    /* left image box */
    .photo-box{
      width:200px;
      min-width:140px;
      height:200px;
      border-radius:10px;
      overflow:hidden;
      background:linear-gradient(180deg,#eef2ff,#fff);
      display:flex;
      align-items:center;
      justify-content:center;
      border:1px solid rgba(15,23,42,0.06);
    }

    .photo-box img{
      width:100%;
      height:100%;
      object-fit:cover;
      display:block;
    }

    /* right content */
    .info{
      flex:1;
      min-width:0;
    }

    .name{
      margin:0 0 6px 0;
      font-size:1.6rem;
      line-height:1.1;
    }
    .surname{
      margin:0 0 12px 0;
      font-size:1.05rem;
      color:var(--muted);
    }

    .description{
      margin-top:6px;
      color:#22314a;
      line-height:1.6;
      font-size:0.98rem;
    }

    /* small screens: stack */
    @media (max-width:640px){
      .profile{flex-direction:column;align-items:center;text-align:center}
      .info{text-align:center}
      .photo-box{width:180px;height:180px}
    }

    /* helper */
    .hint{font-size:0.85rem;color:var(--muted);margin-top:12px}
  </style>
</head>
<body>
  <div class="wrap">
    <div class="card">
      <!-- Contenedor principal: imagen a la izquierda, texto a la derecha -->
      <div class="profile">
        <!-- Recuadro para la imagen -->
        <div class="photo-box" aria-hidden="false">
          <!-- Sustituye "assets/mi-foto.jpg" por la ruta de tu imagen -->
          <img src="assets/mi-foto.png" alt="Foto de perfil">
        </div>

        <!-- Información personal -->
        <div class="info">
          <!-- Nombres y apellidos -->
          <h1 class="fullname">Juan Sebastian Guerrero Ceron</h1>

          <!-- Descripción general -->
          <p class="description">Soy [tu nombre], una persona apasionada por [tus intereses o profesión]. Aquí puedes escribir una breve biografía — por ejemplo: formación académica, ocupación actual, pasatiempos, habilidades principales o cualquier dato que quieras destacar en pocas líneas.</p>

          <p class="hint">Consejo: reemplaza el texto y la imagen en <code>assets/mi-foto.jpg</code> por tus datos reales.</p>
        </div>
      </div>
    </div>
  </div>
</body>
</html>
