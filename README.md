<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>NeoMKFresh — Agencia de Marketing</title>
  <meta name="description" content="NeoMKFresh: agencia de marketing local en Pomabamba. Branding, audio, video, marketing digital y asesoría estratégica."/>
  <style>
    :root {
      --bg:#0f1720; --card:#0b1220; --accent:#38bdf8; --muted:#9aa8bd; --text:#eef2f7;
      --radius:12px;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter,system-ui,Arial,sans-serif;background:linear-gradient(180deg,#071021,#0f1720);color:var(--text)}
    .container{max-width:1100px;margin:0 auto;padding:28px}
    header{display:flex;align-items:center;gap:20px;padding:26px 0}
    .logo-wrap{width:84px;height:84px;border-radius:14px;display:grid;place-items:center;background:linear-gradient(135deg,#0ea5e9,#34d399);box-shadow:0 10px 30px rgba(2,6,23,.6)}
    .brand h1{margin:0;font-size:22px;letter-spacing:.3px}
    .brand p{margin:2px 0 0;color:var(--muted);font-size:14px}

    nav{display:flex;gap:14px;margin-top:6px}
    nav a{color:var(--text);text-decoration:none;padding:8px 12px;border-radius:10px;font-weight:600}
    nav a:hover{background:rgba(255,255,255,.03)}

    .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:center;padding:36px 0}
    .hero h2{font-size:36px;margin:0 0 10px;color:var(--text)}
    .hero p{color:var(--muted);margin:0 0 18px}

    .card{background:linear-gradient(180deg,#071225,#07172a);border:1px solid rgba(255,255,255,.03);padding:18px;border-radius:var(--radius);box-shadow:0 8px 30px rgba(2,6,23,.6)}
    .services{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:18px;margin-top:18px}
    .service img{width:100%;height:140px;object-fit:cover;border-radius:10px;margin-bottom:12px;opacity:.98}
    .service h3{margin:0 0 6px}
    .service p{margin:0;color:var(--muted);font-size:14px}

    form{display:grid;gap:10px;margin-top:12px}
    input,textarea{width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,.04);background:transparent;color:var(--text)}
    button{background:var(--accent);border:none;padding:10px 14px;border-radius:10px;font-weight:700;color:#022;cursor:pointer}

    footer{margin-top:36px;padding:20px 0;color:var(--muted);font-size:14px;text-align:center}

    @media (max-width:920px){
      .hero{grid-template-columns:1fr; padding:22px 0}
      .hero h2{font-size:28px}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo-wrap" aria-hidden="true">
        <!-- Si subes tu logo al repo como img/logo.png reemplaza la img siguiente -->
        <img src="https://images.unsplash.com/photo-1605296867304-46d5465a13f6?w=400&q=80&auto=format&fit=crop" alt="NeoMKFresh logo" style="width:68px;height:68px;border-radius:10px;object-fit:cover">
      </div>
      <div class="brand">
        <h1>NeoMKFresh</h1>
        <p>Agencia de marketing y producción creativa — Pomabamba</p>
        <nav>
          <a href="#nosotros">Nosotros</a>
          <a href="#servicios">Servicios</a>
          <a href="#contacto">Contacto</a>
        </nav>
      </div>
    </header>

    <section class="hero">
      <div>
        <h2>Conectamos tu marca con más clientes, de forma auténtica y medible.</h2>
        <p>NeoMKFresh combina estrategia, creatividad y ejecución local. Diseñamos campañas, producciones de audio y video, y capacitaciones prácticas para que tu negocio sobresalga.</p>

        <div class="card">
          <strong>¿Por qué elegirnos?</strong>
          <ul style="margin:10px 0 0;padding-left:18px;color:var(--muted)">
            <li>Atención presencial en Pomabamba y acompañamiento continuo.</li>
            <li>Estrategias adaptadas a la realidad local y medibles.</li>
            <li>Producción de audio y video con estética minimalista y profesional.</li>
          </ul>
        </div>
      </div>

      <aside class="card">
        <h3 style="margin-top:0">Hablemos de tu proyecto</h3>
        <p style="color:var(--muted);margin-bottom:8px">Escribe tus datos y te respondemos al correo o por WhatsApp.</p>
        <!-- Formulario que abre el correo (mailto) -->
        <form action="mailto:contacto@neomkfresh.pe" method="post" enctype="text/plain">
          <input name="nombre" placeholder="Nombre / Empresa" required>
          <input name="email" type="email" placeholder="Correo electrónico" required>
          <textarea name="mensaje" rows="4" placeholder="Cuéntanos tu proyecto..." required></textarea>
          <button type="submit">Enviar consulta</button>
        </form>
        <p style="color:var(--muted);font-size:13px;margin-top:10px">También puedes contactarnos por WhatsApp: <a href="https://wa.me/51900000000" style="color:var(--accent);text-decoration:none">+51 9XX XXX XXX</a></p>
      </aside>
    </section>

    <section id="servicios">
      <h2 style="margin-bottom:8px">Servicios</h2>
      <div class="services">
        <div class="card service">
          <img src="https://images.unsplash.com/photo-1515378791036-0648a3ef77b2?w=900&q=80&auto=format&fit=crop" alt="Marketing digital minimal">
          <h3>Marketing Digital</h3>
          <p>Campañas estratégicas, gestión de redes y contenido que convierte.</p>
        </div>

        <div class="card service">
          <img src="https://images.unsplash.com/photo-1508830524289-0adcbe822b40?w=900&q=80&auto=format&fit=crop" alt="Branding minimal">
          <h3>Branding & Diseño</h3>
          <p>Identidad visual sobria y coherente que comunica confianza.</p>
        </div>

        <div class="card service">
          <img src="https://images.unsplash.com/photo-1581092334657-f48f4f0b86c2?w=900&q=80&auto=format&fit=crop" alt="Producción audio">
          <h3>Producción de Audio</h3>
          <p>Spots y piezas sonoras con calidad profesional y enfoque local.</p>
        </div>

        <div class="card service">
          <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?w=900&q=80&auto=format&fit=crop" alt="Producción video">
          <h3>Producción de Video</h3>
          <p>Videos minimalistas para redes y presentaciones corporativas.</p>
        </div>

        <div class="card service">
          <img src="https://images.unsplash.com/photo-1633265486064-086b219458ec?w=900&q=80&auto=format&fit=crop" alt="Capacitaciones">
          <h3>Capacitaciones</h3>
          <p>Talleres prácticos en ventas, redes y uso de herramientas digitales.</p>
        </div>

        <div class="card service">
          <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?w=900&q=80&auto=format&fit=crop" alt="Asesoría personalizada">
          <h3>Asesoría Personalizada</h3>
          <p>Diagnóstico, plan de acción y acompañamiento mensual.</p>
        </div>
      </div>
    </section>

    <footer>
      <div style="max-width:900px;margin:0 auto">
        <p style="margin:0 0 8px">© <span id="yr"></span> NeoMKFresh · Página oficial</p>
        <p style="margin:0;color:var(--muted)">Desarrollado para impulsar negocios en Pomabamba — contacto: contacto@neomkfresh.pe</p>
      </div>
    </footer>
  </div>

  <script>
    document.getElementById('yr').textContent = new Date().getFullYear();
  </script>
</body>
</html>

