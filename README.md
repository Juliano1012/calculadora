<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>README - Calculadora Científica</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #111;
      color: #eee;
      padding: 40px;
      line-height: 1.6;
    }

    h1, h2, h3 {
      color: #00f2fe;
    }

    code {
      background-color: #222;
      padding: 2px 6px;
      border-radius: 4px;
      color: #0f0;
    }

    ul {
      margin-left: 20px;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 10px;
    }

    th, td {
      border: 1px solid #444;
      padding: 8px;
      text-align: left;
    }

    th {
      background-color: #333;
    }

    td {
      background-color: #222;
    }

    .highlight {
      color: #ff9500;
    }
  </style>
</head>
<body>
  <h1>📐 Calculadora Científica — README</h1>

  <h2>🧠 Visão Geral</h2>
  <p>Esta é uma calculadora científica moderna desenvolvida com <strong>HTML</strong>, <strong>CSS</strong> e <strong>JavaScript</strong>, projetada para funcionar diretamente no navegador. Ela oferece funções matemáticas básicas e avançadas, incluindo trigonometria, logaritmos, exponenciais, constantes, fatoriais e muito mais.</p>

  <h2>🎨 Interface</h2>
  <ul>
    <li>Fundo preto com corpo da calculadora em cinza escuro.</li>
    <li>Display verde que mostra os cálculos e resultados.</li>
    <li>Botões coloridos para facilitar a identificação:
      <ul>
        <li><span class="highlight">🔴 Vermelho</span>: botão de limpeza (<code>AC</code>)</li>
        <li><span class="highlight">🟠 Laranja</span>: operadores aritméticos (<code>+</code>, <code>−</code>, <code>×</code>, <code>÷</code>)</li>
        <li><span class="highlight">🔵 Azul</span>: botão de resultado (<code>=</code>)</li>
        <li><span class="highlight">⚫ Cinza</span>: números e funções científicas</li>
      </ul>
    </li>
  </ul>

  <h2>🧮 Funcionalidades</h2>
  <h3>🔢 Operações Básicas</h3>
  <ul>
    <li><code>+</code>, <code>−</code>, <code>×</code>, <code>÷</code>: Soma, subtração, multiplicação e divisão.</li>
    <li><code>0–9</code>, <code>.</code>: Entrada de números decimais.</li>
  </ul>

  <h3>🧪 Funções Científicas</h3>
  <table>
    <tr><th>Função</th><th>Descrição</th></tr>
    <tr><td><code>sin</code>, <code>cos</code>, <code>tan</code></td><td>Funções trigonométricas</td></tr>
    <tr><td><code>asin</code>, <code>acos</code>, <code>atan</code></td><td>Funções trigonométricas inversas (ativadas com <code>Inv</code>)</td></tr>
    <tr><td><code>ln</code>, <code>log</code></td><td>Logaritmo natural e logaritmo base 10</td></tr>
    <tr><td><code>exp</code></td><td>Exponencial (<code>e^x</code>)</td></tr>
    <tr><td><code>√</code>, <code>x²</code></td><td>Raiz quadrada e quadrado (com <code>Inv</code>)</td></tr>
    <tr><td><code>xʸ</code></td><td>Potência (<code>x</code> elevado a <code>y</code>)</td></tr>
    <tr><td><code>x!</code></td><td>Fatorial</td></tr>
    <tr><td><code>π</code>, <code>e</code></td><td>Constantes matemáticas</td></tr>
    <tr><td><code>%</code></td><td>Percentual (<code>50%</code> vira <code>50/100</code>)</td></tr>
    <tr><td><code>Ans</code></td><td>Último resultado calculado</td></tr>
  </table>

  <h2>🧭 Modos de Operação</h2>
  <h3>🎛 Deg/Rad</h3>
  <p>Alterna entre <strong>graus</strong> e <strong>radianos</strong> para funções trigonométricas.</p>

  <h3>🔁 Inv</h3>
  <p>Alterna entre funções normais e inversas:</p>
  <ul>
    <li><code>sin</code> ↔ <code>asin</code></li>
    <li><code>cos</code> ↔ <code>acos</code></li>
    <li><code>tan</code> ↔ <code>atan</code></li>
    <li><code>ln</code> ↔ <code>exp</code></li>
    <li><code>log</code> ↔ <code>10ˣ</code></li>
    <li><code>√</code> ↔ <code>x²</code></li>
  </ul>

  <h2>🧠 Lógica JavaScript</h2>
  <ul>
    <li><strong>Display dinâmico</strong>: atualiza conforme o usuário digita.</li>
    <li><strong>Modo Inv</strong>: altera os rótulos e insere funções inversas.</li>
    <li><strong>Modo Deg/Rad</strong>: converte ângulos para radianos se necessário.</li>
    <li><strong>Função <code>calculate()</code></strong>:
      <ul>
        <li>Preprocessa a expressão (ex.: <code>5!</code>, <code>sin(30)</code>).</li>
        <li>Substitui símbolos visuais (<code>×</code>, <code>÷</code>) por operadores reais (<code>*</code>, <code>/</code>).</li>
        <li>Avalia a expressão com <code>eval()</code> em contexto seguro.</li>
        <li>Salva o resultado como <code>Ans</code>.</li>
      </ul>
    </li>
  </ul>

  <h2>🧼 Botões Especiais</h2>
  <ul>
    <li><code>AC</code>: Limpa o display e reinicia a calculadora.</li>
    <li><code>=</code>: Avalia a expressão e mostra o resultado.</li>
    <li><code>Ans</code>: Insere o último resultado calculado.</li>
  </ul>

  <h2>📦 Como Usar</h2>
  <ol>
    <li>Abra o arquivo <code>.html</code> em qualquer navegador moderno.</li>
    <li>Clique nos botões para montar sua expressão.</li>
    <li>Pressione <code>=</code> para calcular.</li>
    <li>Use <code>Ans</code> para reutilizar o último resultado.</li>
    <li>Alterne entre <code>Deg</code> e <code>Rad</code> conforme o tipo de cálculo trigonométrico.</li>
    <li>Use <code>Inv</code> para acessar funções inversas.</li>
  </ol>
