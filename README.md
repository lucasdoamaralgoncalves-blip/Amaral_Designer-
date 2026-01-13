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
    .card {
      background: #111;
      padding: 25px;
      border-radius: 15px;
      border: 1px solid #222;
      margin-bottom: 15px;
    }
    form input, form select {
      width: 100%;
      padding: 14px;
      margin-bottom: 15px;
      border-radius: 10px;
      border: none;
      background: #222;
      color: #fff;
    }
    form button {
      width: 100%;
      padding: 18px;
      border: none;
      border-radius: 50px;
      background: linear-gradient(90deg, #00ffcc, #00ccff);
      color: #000;
      font-weight: 800;
      font-size: 1.1rem;
      cursor: pointer;
    }
    footer {
      text-align: center;
      padding: 30px;
      font-size: 0.9rem;
      color: #888;
    }
  </style>
</head>

<body>

<header>
  <h1>AMARAL DESIGNER</h1>
  <p>Artes esportivas criadas para atletas que querem chamar atenção, se destacar e dar um passo real rumo ao seu sonho.</p>
  <div class="cta">
    <a href="#formulario">CRIAR MINHA ARTE AGORA</a>
  </div>
</header>

<section id="formulario">
  <h2>Formulário de Criação da Arte</h2>

  <form onsubmit="enviarWhatsApp(); return false;">
    <input id="nome" placeholder="Nome completo" required>
    <input id="apelido" placeholder="Apelido (se tiver)">
    <input id="categoria" placeholder="Categoria" required>
    <input id="campeonato" placeholder="Nome do campeonato" required>
    <input id="clubeAtual" placeholder="Clube atual" required>
    <input id="clubeAdv" placeholder="Clube adversário" required>
    <input id="horario" type="time" required>
    <input id="local" placeholder="Local do jogo" required>

    <select id="tipoArte" required>
      <option value="">Tipo de arte</option>
      <option>Story</option>
      <option>Feed</option>
    </select>

    <button type="submit">FINALIZAR PEDIDO E IR PARA O WHATSAPP</button>
  </form>
</section>

<section>
  <h2>Pagamento via Pix</h2>
  <div class="card">
    <strong>Chave Pix:</strong><br>
    51 98941-3011
  </div>
</section>

<footer>
  © AMARAL DESIGNER — Artes Esportivas Profissionais
</footer>

<script>
function enviarWhatsApp() {
  const texto =
`📌 *PEDIDO DE ARTE ESPORTIVA*

👤 Nome: ${nome.value}
⭐ Apelido: ${apelido.value}
🏷️ Categoria: ${categoria.value}
🏆 Campeonato: ${campeonato.value}
⚽ Clube Atual: ${clubeAtual.value}
🆚 Adversário: ${clubeAdv.value}
⏰ Horário: ${horario.value}
📍 Local: ${local.value}
🎨 Tipo de Arte: ${tipoArte.value}

💳 Pagamento via Pix`;

  const url = "https://wa.me/51989413011?text=" + encodeURIComponent(texto);
  window.open(url, "_blank");
}
</script>

</body>
</html>
