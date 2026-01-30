<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <title>Carteira Digital - Layout</title>
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <base href="/confere-carteirinha/">
  <link rel="icon" type="image/x-icon" href="favicon.ico">
  <style>
    /* Estilo inspirado no visual institucional (Cruzeiro do Sul) */
    :root{
      --primary:#004b87; /* tom de azul institucional */
      --primary-700:#00345a;
      --muted:#6b7280;
      --card-bg:#ffffff;
      --page-bg:#f5f8fc;
      --accent-line:#dfeefa;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
      background:linear-gradient(180deg,var(--page-bg),#eef6ff 120%);
      color:var(--primary-700);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .site {
      max-width:920px;
      margin:28px auto;
      padding:16px;
    }

    header.site-header{
      background:linear-gradient(90deg,var(--primary),#006aa6);
      padding:14px 20px;
      border-radius:8px;
      display:flex;
      align-items:center;
      gap:16px;
      box-shadow:0 6px 18px rgba(3,34,63,0.12);
    }
    header.site-header img{height:40px;display:block}
    header.site-header h1{color:#fff;font-size:16px;margin:0;font-weight:700}

    .card {
      margin-top:18px;
      background:var(--card-bg);
      border-radius:8px;
      padding:26px;
      box-shadow:0 8px 30px rgba(15,40,70,0.06);
      border:1px solid var(--accent-line);
    }

    .fields {display:flex;flex-direction:column;gap:14px}
    .row {display:flex;gap:14px;flex-wrap:wrap}
    .col {flex:1;min-width:160px}

    .label{font-size:12px;color:var(--muted);margin-bottom:6px}
    .value{font-size:18px;font-weight:700;color:var(--primary-700);padding:8px 0;border-bottom:2px solid var(--accent-line)}

    .meta {display:flex;justify-content:space-between;color:var(--muted);font-size:13px;margin-top:18px}

    /* Responsive */
    @media (max-width:720px){
      header.site-header{padding:12px}
      .site{padding:12px}
    }
  </style>
</head>
<body>
  <div class="site" role="document">
    <header class="site-header" role="banner" aria-label="Cabeçalho institucional">
      <img alt="Universidade Cruzeiro do Sul" src="https://novoportal.cruzeirodosul.edu.br/static/logos/educacional/flat/cruzeiro-edu.png">
      <h1>Carteira Digital - Cruzeiro do Sul</h1>
    </header>

    <main>
      <article class="card" aria-label="Carteirinha digital">
        <div class="fields">
          <div>
            <div class="label">Nome</div>
            <div class="value">CRISTINA SILVA LIMA DOS SANTOS</div>
          </div>

          <div>
            <div class="label">Curso</div>
            <div class="value">ARTES VISUAIS</div>
          </div>

          <div class="row" aria-hidden="false">
            <div class="col">
              <div class="label">RGM</div>
              <div class="value">548642616</div>
            </div>

            <div class="col">
              <div class="label">CPF</div>
              <div class="value">484.761.598-03</div>
            </div>

            <div class="col">
              <div class="label">Data de validade</div>
              <div class="value">30/06/2027</div>
            </div>
          </div>
        </div>

        <div class="meta" aria-hidden="true">
          <span>Carteirinha Digital</span>
          <span style="visibility:hidden">placeholder</span>
        </div>
      </article>
    </main>
  </div>
</body>
</html>
