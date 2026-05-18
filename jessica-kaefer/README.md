<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Plano de Ação · Jéssica Kaefer · High Level</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet" />
  <style>
    :root {
      --brown-dark:  #2A1A0E;
      --brown-mid:   #3A2214;
      --brown-light: #4E3020;
      --gold:        #C4934A;
      --gold-light:  #D4AC72;
      --gold-pale:   #EED9B0;
      --gold-wash:   #F7EFE0;
      --cream:       #FAF6F0;
      --parchment:   #F2E8D8;
      --text-dark:   #1C1008;
      --text-mid:    #3A2A18;
      --text-soft:   #7A6040;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'DM Sans', sans-serif;
      background: var(--cream);
      color: var(--text-dark);
      font-size: 14px;
      line-height: 1.65;
    }

    /* ── HEADER ── */
    header {
      background: var(--brown-dark);
      color: var(--gold-pale);
      padding: 48px 56px 44px;
      position: relative;
      overflow: hidden;
    }
    header::before {
      content: '';
      position: absolute;
      top: -80px; right: -80px;
      width: 320px; height: 320px;
      border-radius: 50%;
      border: 1px solid rgba(196,147,74,.15);
    }
    header::after {
      content: '';
      position: absolute;
      bottom: -40px; left: 40%;
      width: 180px; height: 180px;
      border-radius: 50%;
      border: 1px solid rgba(196,147,74,.1);
    }
    .eyebrow {
      font-family: 'DM Sans', sans-serif;
      font-size: 10px;
      font-weight: 600;
      letter-spacing: .22em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 18px;
    }
    header h1 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 46px;
      font-weight: 300;
      letter-spacing: -.01em;
      line-height: 1.1;
      color: var(--gold-pale);
      margin-bottom: 6px;
    }
    header h1 em {
      font-style: italic;
      color: var(--gold-light);
    }
    .subtitle {
      font-size: 13px;
      color: rgba(238,217,176,.55);
      font-weight: 300;
      letter-spacing: .04em;
      margin-bottom: 28px;
    }
    .pills {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
    }
    .pill {
      background: rgba(196,147,74,.12);
      border: 1px solid rgba(196,147,74,.3);
      color: var(--gold-light);
      border-radius: 20px;
      padding: 5px 14px;
      font-size: 11px;
      font-weight: 500;
      letter-spacing: .06em;
    }

    /* ── INTRO BANNER ── */
    .intro-banner {
      background: var(--parchment);
      border-left: 4px solid var(--gold);
      padding: 28px 56px;
    }
    .intro-banner p {
      font-family: 'Cormorant Garamond', serif;
      font-size: 18px;
      font-weight: 400;
      font-style: italic;
      color: var(--text-mid);
      line-height: 1.7;
      max-width: 780px;
    }

    /* ── BODY ── */
    .body-wrap {
      max-width: 860px;
      margin: 0 auto;
      padding: 48px 56px 64px;
    }

    /* ── SECTION HEADING ── */
    .sec-head {
      display: flex;
      align-items: baseline;
      gap: 16px;
      margin: 48px 0 24px;
      padding-bottom: 12px;
      border-bottom: 1px solid rgba(196,147,74,.35);
    }
    .sec-num {
      font-family: 'Cormorant Garamond', serif;
      font-size: 36px;
      font-weight: 300;
      color: var(--gold);
      line-height: 1;
      min-width: 36px;
    }
    .sec-title {
      font-family: 'Cormorant Garamond', serif;
      font-size: 22px;
      font-weight: 600;
      color: var(--brown-dark);
      letter-spacing: .01em;
    }

    /* ── SPOTLIGHT ── */
    .spotlight {
      background: var(--brown-dark);
      border-radius: 8px;
      padding: 28px 32px;
      margin-bottom: 18px;
      position: relative;
      overflow: hidden;
    }
    .spotlight::after {
      content: '';
      position: absolute;
      top: -30px; right: -30px;
      width: 120px; height: 120px;
      border-radius: 50%;
      border: 1px solid rgba(196,147,74,.12);
    }
    .spotlight-label {
      font-size: 9.5px;
      font-weight: 600;
      letter-spacing: .2em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 10px;
    }
    .spotlight h3 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 20px;
      font-weight: 600;
      color: var(--gold-pale);
      margin-bottom: 10px;
    }
    .spotlight p {
      font-size: 13.5px;
      color: rgba(238,217,176,.75);
      line-height: 1.7;
    }
    .spotlight p b { color: var(--gold-light); }

    /* ── TABELA ── */
    .tbl-wrap {
      border-radius: 8px;
      overflow: hidden;
      border: 1px solid rgba(196,147,74,.25);
      margin-bottom: 18px;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      font-size: 13px;
    }
    thead tr {
      background: var(--brown-mid);
    }
    th {
      font-size: 10px;
      font-weight: 600;
      letter-spacing: .14em;
      text-transform: uppercase;
      color: var(--gold-light);
      padding: 12px 16px;
      text-align: left;
    }
    td {
      padding: 12px 16px;
      color: var(--text-mid);
      border-bottom: 1px solid rgba(196,147,74,.12);
      vertical-align: top;
    }
    tbody tr:last-child td { border-bottom: none; }
    tbody tr:hover td { background: var(--gold-wash); }
    tbody tr:nth-child(even) td { background: rgba(242,232,216,.35); }
    tbody tr:nth-child(even):hover td { background: var(--gold-wash); }

    .tag {
      display: inline-block;
      border-radius: 12px;
      padding: 3px 10px;
      font-size: 10px;
      font-weight: 600;
      letter-spacing: .06em;
      white-space: nowrap;
    }
    .tag-now  { background: var(--brown-dark); color: var(--gold-light); }
    .tag-week { background: #8a5f1a; color: #fde9b8; }
    .tag-soon { background: var(--parchment); color: var(--text-soft); border: 1px solid rgba(196,147,74,.3); }

    /* ── GRID 2 ── */
    .grid-2 {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 16px;
      margin-bottom: 18px;
    }
    .card {
      border: 1px solid rgba(196,147,74,.3);
      border-radius: 8px;
      padding: 20px;
      background: #fff;
    }
    .card-top {
      display: flex;
      align-items: flex-start;
      gap: 12px;
      margin-bottom: 14px;
    }
    .card-icon {
      width: 36px; height: 36px;
      background: var(--parchment);
      border-radius: 8px;
      display: flex; align-items: center; justify-content: center;
      font-size: 16px;
      flex-shrink: 0;
    }
    .card-icon.gold { background: var(--brown-dark); }
    .card-kicker {
      font-size: 9.5px;
      font-weight: 600;
      letter-spacing: .15em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 3px;
    }
    .card-title {
      font-family: 'Cormorant Garamond', serif;
      font-size: 16px;
      font-weight: 600;
      color: var(--text-dark);
    }
    .card-list {
      list-style: none;
      padding: 0;
    }
    .card-list li {
      font-size: 12.5px;
      color: var(--text-mid);
      padding: 5px 0;
      border-bottom: 1px solid rgba(196,147,74,.1);
      padding-left: 14px;
      position: relative;
    }
    .card-list li:last-child { border-bottom: none; }
    .card-list li::before {
      content: '—';
      position: absolute;
      left: 0;
      color: var(--gold);
      font-size: 10px;
    }

    /* ── CARD FULL ── */
    .card-full {
      border: 1px solid var(--gold);
      border-radius: 8px;
      overflow: hidden;
      margin-bottom: 18px;
    }
    .card-full-head {
      background: var(--brown-dark);
      display: flex;
      align-items: center;
      gap: 12px;
      padding: 14px 20px;
    }
    .card-full-icon { font-size: 18px; }
    .card-full-title {
      font-family: 'Cormorant Garamond', serif;
      font-size: 17px;
      font-weight: 600;
      color: var(--gold-pale);
    }
    .card-full-body {
      padding: 16px 20px;
      font-size: 13.5px;
      color: var(--text-mid);
      line-height: 1.7;
      background: #fff;
    }
    .card-full-body b { color: var(--brown-dark); }

    /* ── FUNIL ── */
    .funnel-wrap {
      border-radius: 8px;
      overflow: hidden;
      margin-bottom: 18px;
      border: 1px solid rgba(196,147,74,.25);
    }
    .funnel-row {
      display: flex;
      align-items: stretch;
    }
    .funnel-row:nth-child(even) .funnel-left { background: var(--brown-mid); }
    .funnel-row:nth-child(even) .funnel-right { background: rgba(242,232,216,.4); }
    .funnel-left {
      background: var(--brown-dark);
      padding: 18px 20px;
      min-width: 100px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
    }
    .funnel-price {
      font-family: 'Cormorant Garamond', serif;
      font-size: 18px;
      font-weight: 700;
      color: var(--gold-light);
    }
    .funnel-tier {
      font-size: 9px;
      letter-spacing: .15em;
      text-transform: uppercase;
      color: rgba(238,217,176,.5);
      margin-top: 4px;
    }
    .funnel-right {
      flex: 1;
      background: #fff;
      padding: 16px 20px;
      border-bottom: 1px solid rgba(196,147,74,.15);
    }
    .funnel-row:last-child .funnel-right { border-bottom: none; }
    .funnel-name {
      font-family: 'Cormorant Garamond', serif;
      font-size: 16px;
      font-weight: 600;
      color: var(--text-dark);
      margin-bottom: 4px;
    }
    .funnel-desc {
      font-size: 12.5px;
      color: var(--text-soft);
      line-height: 1.55;
    }

    /* ── CHECKLIST ── */
    .checklist-wrap {
      border: 1px solid rgba(196,147,74,.3);
      border-radius: 8px;
      overflow: hidden;
      margin-bottom: 18px;
    }
    .checklist-head {
      background: var(--parchment);
      padding: 12px 20px;
      font-size: 10px;
      font-weight: 600;
      letter-spacing: .16em;
      text-transform: uppercase;
      color: var(--text-soft);
      border-bottom: 1px solid rgba(196,147,74,.2);
    }
    .cl-item {
      display: flex;
      align-items: flex-start;
      gap: 14px;
      padding: 13px 20px;
      border-bottom: 1px solid rgba(196,147,74,.1);
      cursor: pointer;
      transition: background .15s;
    }
    .cl-item:last-child { border-bottom: none; }
    .cl-item:hover { background: var(--gold-wash); }
    .cl-item.done { background: rgba(196,147,74,.08); }
    .cl-box {
      width: 18px; height: 18px;
      border: 1.5px solid var(--gold);
      border-radius: 4px;
      flex-shrink: 0;
      margin-top: 2px;
      transition: all .15s;
      display: flex; align-items: center; justify-content: center;
    }
    .cl-item.done .cl-box {
      background: var(--gold);
    }
    .cl-item.done .cl-box::after {
      content: '✓';
      color: #fff;
      font-size: 11px;
      font-weight: 700;
    }
    .cl-text {
      font-size: 13px;
      color: var(--text-mid);
      line-height: 1.55;
    }
    .cl-item.done .cl-text {
      text-decoration: line-through;
      color: var(--text-soft);
    }
    .cl-text b { color: var(--text-dark); }
    .cl-item.done .cl-text b { color: var(--text-soft); }

    /* ── FOOTER ── */
    footer {
      background: var(--brown-dark);
      padding: 24px 56px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 12px;
    }
    .footer-brand {
      font-family: 'Cormorant Garamond', serif;
      font-size: 18px;
      font-weight: 700;
      letter-spacing: .08em;
      color: var(--gold);
    }
    .footer-meta {
      font-size: 11px;
      color: rgba(238,217,176,.5);
      letter-spacing: .06em;
    }

    /* ── PRINT ── */
    @media print {
      body { background: #fff; }
      header, footer { -webkit-print-color-adjust: exact; print-color-adjust: exact; }
      .spotlight, .tbl-wrap, .funnel-wrap, .card, .card-full, .checklist-wrap {
        -webkit-print-color-adjust: exact; print-color-adjust: exact;
        break-inside: avoid;
      }
      .body-wrap { padding: 32px 40px; }
    }

    @media (max-width: 640px) {
      header, .intro-banner, footer { padding-left: 24px; padding-right: 24px; }
      .body-wrap { padding: 32px 24px; }
      header h1 { font-size: 34px; }
      .grid-2 { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>

<!-- ═══════════════ HEADER ═══════════════ -->
<header>
  <div class="eyebrow">High Level · Método Governe · Plano de Ação</div>
  <h1>Jéssica <em>Kaefer</em></h1>
  <p class="subtitle">Mentora de Negócios &amp; Estrategista · Método Governe</p>
  <div class="pills">
    <span class="pill">11.05.2026</span>
    <span class="pill">Refinamento Estratégico</span>
    <span class="pill">Reposicionamento &amp; Ativação de Vendas</span>
  </div>
</header>

<!-- ═══════════════ INTRO BANNER ═══════════════ -->
<div class="intro-banner">
  <p>
    Este encontro marcou a virada oficial de posicionamento de Jéssica: do universo Mary K para a construção de uma autoridade própria como mentora estrategista. O foco central foi estruturar o <b>Método Governe</b> como pilar do negócio, definir a escada de produtos e lançar a próxima imersão com intenção de conversão em mentoria <em>high ticket</em>.
  </p>
</div>

<!-- ═══════════════ BODY ═══════════════ -->
<div class="body-wrap">

  <!-- ─── 01 · CONTEXTO E REPOSICIONAMENTO ─── -->
  <div class="sec-head">
    <div class="sec-num">01</div>
    <div class="sec-title">Contexto &amp; Reposicionamento</div>
  </div>

  <div class="spotlight">
    <div class="spotlight-label">Momento atual · Diagnóstico</div>
    <h3>Da Mary K para a Mentoria Própria</h3>
    <p>
      Jéssica passou por um processo intenso de <b>transição profissional</b>. Abriu e vendeu uma empresa de higienização com sucesso (R$ 15 mil após 10 meses), comprovou sua capacidade de estruturar negócios e tomou a decisão de encerrar o envolvimento ativo com a Mary K. O evento <b>"Governe"</b> — com 50 pessoas e 3 mentorias vendidas a R$ 2.500 — foi a prova de que o novo posicionamento funciona.
    </p>
  </div>

  <div class="grid-2">
    <div class="card">
      <div class="card-top">
        <div class="card-icon">✅</div>
        <div>
          <div class="card-kicker">O que permanece</div>
          <div class="card-title">Mary K · Manutenção Estratégica</div>
        </div>
      </div>
      <ul class="card-list">
        <li>Manter afiliação apenas para receber bônus mensais</li>
        <li>Não renunciar formalmente ao status de nacional</li>
        <li>Agir com discrição — sem criticar publicamente</li>
        <li>Assistentes virtuais atendem a área; Jéssica não se envolve</li>
        <li>Bônus mensais compõem o orçamento familiar no curto prazo</li>
      </ul>
    </div>
    <div class="card">
      <div class="card-top">
        <div class="card-icon gold">🚀</div>
        <div>
          <div class="card-kicker">O que é o foco agora</div>
          <div class="card-title">Negócio Próprio · Método Governe</div>
        </div>
      </div>
      <ul class="card-list">
        <li>Mentoria individual como produto principal</li>
        <li>Eventos presenciais como funil de conversão</li>
        <li>Posicionamento como mentora estrategista</li>
        <li>Método estruturado nos pilares: Atrair · Converter · Gerir</li>
        <li>Perfil comportamental como diferencial do método</li>
      </ul>
    </div>
  </div>

  <!-- ─── 02 · ESTRUTURA DE PRODUTOS E PREÇOS ─── -->
  <div class="sec-head">
    <div class="sec-num">02</div>
    <div class="sec-title">Escada de Produtos &amp; Precificação</div>
  </div>

  <div class="spotlight">
    <div class="spotlight-label">Lógica de Funil · Princípio Central</div>
    <h3>Eventos Baratos → Mentoria High Ticket</h3>
    <p>
      Eventos presenciais são o funil que <b>mais converte</b>, mas precisam ser estruturados com intenção de vender o próximo nível. Ingressos baratos atraem mais pessoas; mais pessoas = mais chances de converter em mentoria de <b>R$ 4.000 a R$ 5.000</b>. O evento não é a receita principal — é a porta de entrada.
    </p>
  </div>

  <div class="funnel-wrap">
    <div class="funnel-row">
      <div class="funnel-left">
        <div class="funnel-price">R$ 247</div>
        <div class="funnel-tier">Entrada</div>
      </div>
      <div class="funnel-right">
        <div class="funnel-name">Imersão Governe · "Vista Sua Capa"</div>
        <div class="funnel-desc">Evento presencial de 1 dia para empreendedoras. Foco em desenvolvimento pessoal + negócios. Meta: 6 de junho. Objetivo: encher o evento e converter em mentoria. Preço baixo = volume de pessoas = conversão no pit de vendas.</div>
      </div>
    </div>
    <div class="funnel-row">
      <div class="funnel-left">
        <div class="funnel-price">R$ 950</div>
        <div class="funnel-tier">Grupo</div>
      </div>
      <div class="funnel-right">
        <div class="funnel-name">Mentoria em Grupo · Método Governe</div>
        <div class="funnel-desc">1 encontro semanal em grupo + abertura semanal do WhatsApp para dúvidas. Acesso limitado (sem abertura individual excessiva). Gera desejo pela mentoria individual. Valor cresce proporcionalmente ao aumento da mentoria individual.</div>
      </div>
    </div>
    <div class="funnel-row">
      <div class="funnel-left">
        <div class="funnel-price">R$ 3.500</div>
        <div class="funnel-tier">Individual</div>
      </div>
      <div class="funnel-right">
        <div class="funnel-name">Mentoria Individual · Próxima Venda</div>
        <div class="funnel-desc">Valor para a próxima cliente (empreendedora de festas em potencial). Encontros quinzenais — tempo de implementação entre sessões. Caminho para chegar ao valor de mercado ideal.</div>
      </div>
    </div>
    <div class="funnel-row">
      <div class="funnel-left">
        <div class="funnel-price">R$ 5.000+</div>
        <div class="funnel-tier">Referência</div>
      </div>
      <div class="funnel-right">
        <div class="funnel-name">Mentoria Individual · Valor de Mercado</div>
        <div class="funnel-desc">Meta de precificação para a mentoria individual de 3 meses. Mais acesso à mentora, mais personalização, mais resultado. Valor que posiciona Jéssica no segmento premium do mercado.</div>
      </div>
    </div>
    <div class="funnel-row">
      <div class="funnel-left">
        <div class="funnel-price">Futuro</div>
        <div class="funnel-tier">Escala</div>
      </div>
      <div class="funnel-right">
        <div class="funnel-name">Modelo Híbrido · Individual + Grupo Anual</div>
        <div class="funnel-desc">Após consolidar mentorias individuais: criar modelo como o da High Level — parte individual, parte em grupo, duração de 1 ano. Próximo nível de escala sem perder a qualidade de entrega.</div>
      </div>
    </div>
  </div>

  <!-- ─── 03 · ESTRUTURAÇÃO DO MÉTODO GOVERNE ─── -->
  <div class="sec-head">
    <div class="sec-num">03</div>
    <div class="sec-title">Estruturação do Método Governe</div>
  </div>

  <div class="card-full">
    <div class="card-full-head">
      <div class="card-full-icon">🏛️</div>
      <div class="card-full-title">Os Pilares do Método Governe</div>
    </div>
    <div class="card-full-body">
      O método se estrutura em três pilares: <b>Atrair</b> (como o público encontra e se conecta com Jéssica), <b>Converter</b> (como transformar interesse em cliente pagante) e <b>Gerir</b> (como entregar resultado e fidelizar). O <b>perfil comportamental</b> é o diferencial que atravessa todos os pilares — é a identidade do método e o que o torna único no mercado.
    </div>
  </div>

  <div class="grid-2">
    <div class="card">
      <div class="card-top">
        <div class="card-icon">📓</div>
        <div>
          <div class="card-kicker">Ferramenta de Organização</div>
          <div class="card-title">Notion · Central de Materiais</div>
        </div>
      </div>
      <ul class="card-list">
        <li>Centralizar toda a estrutura do método</li>
        <li>Organizar materiais de apoio para mentoradas</li>
        <li>Versão gratuita suficiente para o início</li>
        <li>Renata enviará modelos de Notion como base</li>
        <li>Um único lugar para tudo: método, clientes, cronograma</li>
      </ul>
    </div>
    <div class="card">
      <div class="card-top">
        <div class="card-icon gold">🎯</div>
        <div>
          <div class="card-kicker">Foco Estratégico</div>
          <div class="card-title">Uma Coisa de Cada Vez</div>
        </div>
      </div>
      <ul class="card-list">
        <li>Foco único: Governe + Mentorias individuais</li>
        <li>Não dispersar em mentoria para casais agora</li>
        <li>Não criar treinamentos empresariais no momento</li>
        <li>Reposicionamento exige clareza de nicho</li>
        <li>Depois de consolidado, expandir com estratégia</li>
      </ul>
    </div>
  </div>

  <!-- ─── 04 · IMERSÃO GOVERNE · PRÓXIMO EVENTO ─── -->
  <div class="sec-head">
    <div class="sec-num">04</div>
    <div class="sec-title">Imersão Governe · Lançamento Imediato</div>
  </div>

  <div class="spotlight">
    <div class="spotlight-label">Próxima Ação · Alta Prioridade</div>
    <h3>Imersão Governe: "Vista Sua Capa"</h3>
    <p>
      Evento presencial de 1 dia para empreendedoras. Data prevista: <b>6 de junho</b>. Meta de receita: <b>R$ 30.000</b>. O lançamento deve acontecer <b>hoje</b> — iniciar convite dos contatos quentes imediatamente. Ingresso a <b>R$ 247</b> para maximizar volume de participantes e aumentar a conversão em mentoria no pit de vendas.
    </p>
  </div>

  <div class="tbl-wrap">
    <table>
      <thead>
        <tr>
          <th>Elemento do Evento</th>
          <th>Descrição / Estratégia</th>
          <th>Prioridade</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><b>Lançamento do evento</b></td>
          <td>Lançar hoje. Iniciar convite para contatos quentes imediatamente</td>
          <td><span class="tag tag-now">Agora</span></td>
        </tr>
        <tr>
          <td><b>Preço do ingresso</b></td>
          <td>R$ 247 — baixo para atrair volume e maximizar conversão em mentoria</td>
          <td><span class="tag tag-now">Agora</span></td>
        </tr>
        <tr>
          <td><b>Lineup e cronograma</b></td>
          <td>Renata cria cronograma minuto a minuto usando estrutura Atrair · Converter · Gerir</td>
          <td><span class="tag tag-now">Agora</span></td>
        </tr>
        <tr>
          <td><b>Pit de vendas</b></td>
          <td>Renata define o momento ideal (antes ou depois do almoço). Oferta: mentoria R$ 4.000–5.000</td>
          <td><span class="tag tag-week">Esta semana</span></td>
        </tr>
        <tr>
          <td><b>Estrutura de conteúdo</b></td>
          <td>Desenvolvimento pessoal + negócios. Perfil comportamental como âncora do método</td>
          <td><span class="tag tag-week">Esta semana</span></td>
        </tr>
        <tr>
          <td><b>Meta financeira</b></td>
          <td>R$ 30.000 — provenientes de conversões em mentoria individual no evento</td>
          <td><span class="tag tag-soon">Em breve</span></td>
        </tr>
      </tbody>
    </table>
  </div>

  <div class="card-full">
    <div class="card-full-head">
      <div class="card-full-icon">🗓️</div>
      <div class="card-full-title">Encontro Presencial High Level · Agosto 2026</div>
    </div>
    <div class="card-full-body">
      Jéssica confirmou participação no encontro presencial da High Level em <b>Alphaville, São Paulo</b>, nos dias <b>20, 21 e 22 de agosto</b>. Ela planeja levar uma amiga corretora de imóveis — potencial mentorada. Organizar presença pessoal e logística para comparecer ao evento.
    </div>
  </div>

  <!-- ─── 05 · PLANO DE AÇÃO · PRÓXIMOS PASSOS ─── -->
  <div class="sec-head">
    <div class="sec-num">05</div>
    <div class="sec-title">Plano de Ação · Próximos Passos</div>
  </div>

  <div class="tbl-wrap">
    <table>
      <thead>
        <tr>
          <th>Responsável</th>
          <th>Ação</th>
          <th>Prazo</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><b>Jéssica</b></td>
          <td>Lançar Imersão Governe e iniciar convite de contatos quentes</td>
          <td><span class="tag tag-now">Hoje</span></td>
        </tr>
        <tr>
          <td><b>Jéssica</b></td>
          <td>Enviar estrutura base do Método Governe para Renata analisar</td>
          <td><span class="tag tag-now">Hoje</span></td>
        </tr>
        <tr>
          <td><b>Renata</b></td>
          <td>Criar lineup e cronograma minuto a minuto da imersão</td>
          <td><span class="tag tag-week">Esta semana</span></td>
        </tr>
        <tr>
          <td><b>Renata</b></td>
          <td>Definir momento ideal do pit de vendas na imersão (antes ou depois do almoço)</td>
          <td><span class="tag tag-week">Esta semana</span></td>
        </tr>
        <tr>
          <td><b>Renata</b></td>
          <td>Enviar modelos de Notion e materiais de apoio do acervo</td>
          <td><span class="tag tag-week">Esta semana</span></td>
        </tr>
        <tr>
          <td><b>Jéssica</b></td>
          <td>Implementar estrutura no Notion — centralizar todas as informações</td>
          <td><span class="tag tag-soon">Em breve</span></td>
        </tr>
        <tr>
          <td><b>Jéssica</b></td>
          <td>Agendar próxima cliente de mentoria (empreendedora de festas) por R$ 3.500</td>
          <td><span class="tag tag-soon">Em breve</span></td>
        </tr>
        <tr>
          <td><b>Jéssica</b></td>
          <td>Confirmar e organizar presença no evento presencial de agosto em SP</td>
          <td><span class="tag tag-soon">Em breve</span></td>
        </tr>
        <tr>
          <td><b>Jéssica</b></td>
          <td>Convidar amiga corretora de imóveis para o evento presencial de agosto</td>
          <td><span class="tag tag-soon">Em breve</span></td>
        </tr>
      </tbody>
    </table>
  </div>

  <!-- ─── 06 · CHECKLIST DE EXECUÇÃO ─── -->
  <div class="sec-head">
    <div class="sec-num">06</div>
    <div class="sec-title">Checklist de Execução</div>
  </div>

  <div class="checklist-wrap">
    <div class="checklist-head">Marque conforme for avançando</div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Lançar Imersão Governe hoje</b> — publicar nas redes, enviar mensagem para contatos quentes e abrir inscrições a R$ 247</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Enviar estrutura do Método Governe para Renata</b> — compartilhar o que já está montado dos pilares Atrair, Converter e Gerir</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Receber e implementar modelos de Notion</b> — centralizar método, clientes e materiais em um único lugar</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Receber o lineup da imersão</b> — cronograma minuto a minuto com o momento do pit de vendas definido</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Vender mentoria para empreendedora de festas</b> — valor R$ 3.500, encontros quinzenais, 3 meses de acompanhamento</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Manter estrutura Mary K ativa sem envolvimento</b> — assistentes virtuais atendem a área, bônus continuam chegando, sem posts nem movimentação pública</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Manter foco único: Governe + Mentorias</b> — não iniciar projetos paralelos (casais, empresarial) neste momento de reposicionamento</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Confirmar logística para agosto</b> — organizar presença no encontro presencial High Level em Alphaville (20, 21 e 22/08)</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Convidar amiga corretora</b> — levar para o evento presencial de agosto como potencial mentorada</div>
    </div>

    <div class="cl-item" onclick="toggle(this)">
      <div class="cl-box"></div>
      <div class="cl-text"><b>Atingir meta de R$ 30.000</b> na Imersão Governe através de conversões em mentoria individual no pit de vendas</div>
    </div>
  </div>

</div><!-- /body-wrap -->

<!-- ═══════════════ FOOTER ═══════════════ -->
<footer>
  <div class="footer-brand">HIGH LEVEL</div>
  <div class="footer-meta">Mentora Renata Amadeu &nbsp;·&nbsp; 11.05.2026 &nbsp;·&nbsp; Refinamento · Jéssica Kaefer</div>
</footer>

<script>
  function toggle(el) {
    el.classList.toggle('done');
  }
</script>

</body>
</html>
