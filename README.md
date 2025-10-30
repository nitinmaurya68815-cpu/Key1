


<!doctype html>
<html lang="hi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>VIP MOD — Dashboard (Static)</title>
  <style>
    /* Background neon gradient */
    :root{
      --bg1: #0f0c29;
      --bg2: #302b63;
      --accent: #00ffd5;
      --neon: #00e6ff;
      --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.02);
    }
    html,body{height:100%;margin:0;font-family:Inter,ui-sans-serif,system-ui,Segoe UI,Roboto,"Helvetica Neue",Arial;}
    body{
      background: radial-gradient(1000px 600px at 10% 10%, rgba(0,255,213,0.06), transparent 8%),
                  radial-gradient(800px 500px at 90% 90%, rgba(0,150,255,0.05), transparent 10%),
                  linear-gradient(120deg,var(--bg1),var(--bg2));
      color:#e6f7ff;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding:48px;
      box-sizing:border-box;
    }

    /* Container */
    .wrap{
      max-width:1100px;
      margin:0 auto;
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:28px;
      align-items:start;
    }

    /* Card style */
    .card{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:16px;
      padding:20px;
      box-shadow: 0 8px 30px rgba(2,6,23,0.6);
      border:1px solid rgba(255,255,255,0.04);
      backdrop-filter: blur(6px) saturate(120%);
    }

    header{
      display:flex;
      justify-content:space-between;
      align-items:center;
      margin-bottom:18px;
    }
    .brand{
      display:flex;
      gap:12px;
      align-items:center;
    }
    .logo{
      width:60px;height:60px;border-radius:12px;
      background: linear-gradient(135deg, rgba(0,230,255,0.08), rgba(0,255,180,0.06));
      display:flex;align-items:center;justify-content:center;
      font-weight:700;font-size:20px;color:var(--neon);
      box-shadow: 0 0 18px rgba(0,230,255,0.08), 0 0 48px rgba(0,150,255,0.03) inset;
      border:1px solid rgba(0,230,255,0.08);
      text-transform:uppercase;
    }
    h1{font-size:20px;margin:0;}
    p.lead{margin:0;color:rgba(230,247,255,0.75);font-size:13px}

    /* Neon headline */
    .neon-title{
      font-size:28px;
      font-weight:700;
      color: #e6ffff;
      text-shadow:
        0 0 6px rgba(0,230,255,0.28),
        0 0 18px rgba(0,180,255,0.12),
        0 6px 30px rgba(2,8,20,0.6);
      letter-spacing:1px;
      margin:0 0 10px 0;
    }

    /* Feature list */
    .features{display:flex;flex-wrap:wrap;gap:10px}
    .feat{
      min-width:120px;
      background:linear-gradient(180deg,var(--glass),var(--glass-2));
      border-radius:10px;padding:10px 12px;
      border:1px solid rgba(0,255,210,0.06);
      box-shadow: 0 6px 18px rgba(0,0,0,0.45);
      font-weight:600;color:#bffaf7;font-size:13px;
      display:flex;justify-content:space-between;align-items:center;
    }
    .on{color:#b5ffcd;text-shadow:0 0 8px rgba(0,230,180,0.12)}
    .off{color:#ffb3b3;opacity:0.9;text-shadow:0 0 6px rgba(255,80,80,0.08)}

    /* Right column */
    .side .btn{
      display:inline-block;padding:10px 14px;border-radius:10px;
      text-decoration:none;font-weight:700;
      border:1px solid rgba(255,255,255,0.06);
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      margin-bottom:10px;
    }

    .links a{display:block;padding:10px 12px;border-radius:10px;margin-bottom:10px;text-decoration:none;color:inherit;border:1px solid rgba(255,255,255,0.03)}
    .links a:hover{transform:translateY(-3px);transition:all .18s ease}

    table{width:100%;border-collapse:collapse;margin-top:12px}
    th,td{padding:10px;text-align:left;font-size:13px;border-bottom:1px dashed rgba(255,255,255,0.03)}
    th{font-size:12px;color:rgba(255,255,255,0.7);text-transform:uppercase;letter-spacing:0.6px}

    .center{display:flex;gap:10px;align-items:center}
    .download{
      padding:10px 12px;border-radius:10px;background:linear-gradient(90deg,#001e2a,#00394b);
      color:#aef0ff;text-decoration:none;font-weight:700;border:1px solid rgba(0,250,220,0.08);
      box-shadow:0 8px 30px rgba(0,30,40,0.6), 0 0 18px rgba(0,200,230,0.06) inset;
    }

    footer{margin-top:20px;color:rgba(255,255,255,0.5);font-size:13px;text-align:center}
    @media(max-width:980px){
      .wrap{grid-template-columns:1fr; padding:12px}
      .logo{width:48px;height:48px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <main class="card">
      <header>
        <div class="brand">
          <div class="logo">VIP</div>
          <div>
            <h1 class="neon-title">VIP MOD — Dashboard</h1>
            <p class="lead">Static preview of your site — data shown is sample (read-only)</p>
          </div>
        </div>
        <div style="text-align:right">
          <div style="font-size:12px;color:rgba(255,255,255,0.6)">Status</div>
          <div style="font-weight:800;color:#9cffb8">Online</div>
        </div>
      </header>

      <section>
        <h3 style="margin:0 0 8px 0">Features (Static)</h3>
        <div class="features">
          <div class="feat"><span>ESP</span><span class="on">ON</span></div>
          <div class="feat"><span>Item</span><span class="on">ON</span></div>
          <div class="feat"><span>SilentAim</span><span class="on">ON</span></div>
          <div class="feat"><span>AIM</span><span class="on">ON</span></div>
          <div class="feat"><span>BulletTrack</span><span class="on">ON</span></div>
          <div class="feat"><span>Memory</span><span class="on">ON</span></div>
          <div class="feat"><span>Floating</span><span class="on">ON</span></div>
          <div class="feat"><span>Setting</span><span class="on">ON</span></div>
        </div>
      </section>

      <section style="margin-top:18px">
        <h3 style="margin:0 0 8px 0">Key Info / Admin</h3>
        <table>
          <tr><th>Field</th><th>Value (sample)</th></tr>
          <tr><td>Mod Name</td><td>VIP MOD</td></tr>
          <tr><td>Admin Username</td><td>admin</td></tr>
          <tr><td>Admin Email</td><td>support@aloneboy.com</td></tr>
          <tr><td>Default Expiration</td><td>2050-01-01</td></tr>
          <tr><td>Lib File</td><td>lib.so (555 KB)</td></tr>
        </table>
        <div style="margin-top:12px" class="center">
          <a class="download" href="#" title="Download lib (static)">Download lib.so</a>
          <span style="font-size:13px;color:rgba(255,255,255,0.6)">| Use server-side to serve real file</span>
        </div>
      </section>

      <footer>
        Static site generated from DB export — to make it dynamic (login, key checks, downloads), server-side PHP + MySQL chahiye.
      </footer>
    </main>

    <aside class="card side">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
        <div>
          <div style="font-size:12px;color:rgba(255,255,255,0.6)">Welcome,</div>
          <div style="font-weight:800">Owner / Admin</div>
        </div>
        <div style="text-align:right">
          <div style="font-size:12px;color:rgba(255,255,255,0.6)">Uptime</div>
          <div style="font-weight:700">99.99%</div>
        </div>
      </div>

      <div class="links">
        <a href="https://youtube.com/@sanatanigamer90?si=gywPA0dIIy6Y5652" target="_blank" rel="noopener">▶ YouTube: sanatanigamer90</a>
        <a href="https://youtube.com/@nitinnm4627?si=81BNKXJj9pfYSiua" target="_blank" rel="noopener">▶ YouTube: nitinnm4627</a>
        <a href="https://t.me/+MVN" target="_blank" rel="noopener">▶ Telegram Channel</a>
      </div>

      <div style="margin-top:14px">
        <a class="btn" href="#" onclick="alert('Static: register functionality requires server-side code')">Register (Static)</a>
        <a class="btn" href="#" onclick="alert('Static: admin login requires server-side code')">Admin Login (Static)</a>
      </div>

      <div style="margin-top:16px">
        <h4 style="margin:0 0 8px 0">Referral / Credits</h4>
        <table>
          <tr><th>Code</th><th>Reward</th></tr>
          <tr><td>REF-EXAMPLE</td><td>0</td></tr>
        </table>
      </div>
    </aside>
  </div>
</body>
</html>
