<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AMARAL DESIGNER | Artes Esportivas</title>

  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;800&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background: radial-gradient(circle at top, #1b1b1b, #000);
      color: #ffffff;
    }

    header {
      padding: 80px 20px;
      text-align: center;
    }

    header h1 {
      font-size: 3rem;
      font-weight: 800;
      color: #00ffcc;
    }

    header p {
      max-width: 700px;
      margin: 20px auto;
      font-size: 1.2rem;
      color: #dddddd;
    }

    .cta {
      margin-top: 30px;
    }

    .cta a {
      background: linear-gradient(90deg, #00ffcc, #00ccff);
      padding: 16px 36px;
      border-radius: 50px;
      color: #000;
      font-weight: 700;
      text-decoration: none;
      font-size: 1.1rem;
    }

    section {
      padding: 70px 20px;
      max-width: 1000px;
      margin: auto;
    }

    section h2 {
      font-size: 2.2rem;
      margin-bottom: 20px;
      color: #00ffcc;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background: #111111;
      padding: 25px;
      border-radius: 15px;
      border: 1px solid #222222;
    }

    form input,
    form select {
      width: 100%;
      padding: 14px;
      margin-bottom: 15px;
      border-radius: 10px;
      border: none;
      background: #222222;
      color: #ffffff;
    }

    form input[type="file"] {
      background: #111111;
    }

    form button {
      width: 100%;
      padding: 18px;
      border: none;
      border-radius: 50px;
      background: linear-gradient(90deg, #00ffcc, #00ccff);
      color: #000000;
      font-weight: 800;
      font-size: 1.1rem;
      cursor: pointer;
    }

    footer {
      text-align: center;
      padding: 30px;
      font-size: 0.9rem;
      color: #888888;
    }
  </style>
</head>

<body>

  <header>
    <h1>AMARAL DESIGNER</h1>
    <p>
      Artes esportivas criadas para atletas que querem chamar atenção,
      se destacar e dar um passo real rumo ao seu sonho.
    </p>

    <div class="cta">
      <a href="#formulario">CRIAR MINHA ARTE AGORA</a>
    </div>
  </header>

  <section>
    <h2>Por que investir na sua imagem?</h2>

    <div class="grid">
      <div class="card">📸 Visual profissional que chama atenção</div>
      <div class="card">⚽ Destaque para clubes, campeonatos e redes sociais</div>
      <div class="card">🔥 Sua imagem no nível do seu talento</div>
    </div>
  </section>

  <section id="formulario">
    <h2>Formulário de Criação da Arte</h2>

    <form>
      <input type="text" placeholder="Nome completo" required>
      <input type="text" placeholder="Apelido (se tiver)">
      <input type="text" placeholder="Categoria" required>
      <input type="text" placeholder="Nome do campeonato" required>
      <input type="text" placeholder="Clube atual" required>
      <input type="text" placeholder="Clube adversário" required>
      <input type="time" required>
      <input type="text" placeholder="Local do jogo" required>

      <select required>
        <option value="">Tipo de arte</option>
        <option>Story</option>
        <option>Feed</option>
      </select>

      <input type="file" accept="image/*" multiple required>

      <button type="submit">
        FINALIZAR PEDIDO E PAGAR VIA PIX
      </button>
    </form>
  </section>

  <section>
    <h2>Pagamento via Pix</h2>
    <p>
      Após o envio do formulário, realize o pagamento via Pix para iniciar
      a produção da sua arte.
    </p>

    <div class="card">
      <strong>Chave Pix:</strong><br>
      51 98941-3011
    </div>
  </section>

  <footer>
    © AMARAL DESIGNER — Artes Esportivas Profissionais
  </footer>

</body>
</html>
