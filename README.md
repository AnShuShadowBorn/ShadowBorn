<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Shadow Born - Tripulação Sombria</title>
<style>
  /* Reset básico */
  * {
    margin: 0; padding: 0; box-sizing: border-box;
  }
  body, html {
    height: 100%;
    font-family: Arial, Helvetica, sans-serif;
    background: linear-gradient(#000000, #111111);
    color: #eee;
    overflow-x: hidden;
    position: relative;
  }
  /* Fundo com neblina animada */
  .nebula {
    position: fixed;
    top: 0; left: 0; width: 100%; height: 100%;
    background: radial-gradient(circle at 30% 30%, rgba(150,150,180,0.3), transparent 60%),
                radial-gradient(circle at 70% 70%, rgba(80,80,110,0.4), transparent 50%);
    animation: nebAnim 40s linear infinite;
    z-index: 0;
    filter: blur(60px);
  }
  @keyframes nebAnim {
    0% {background-position: 30% 30%, 70% 70%;}
    50% {background-position: 35% 35%, 65% 65%;}
    100% {background-position: 30% 30%, 70% 70%;}
  }
  /* Silhuetas barcos e caveiras */
  .silhouettes {
    position: fixed;
    bottom: 0; left: 0; width: 100%; height: 150px;
    background:
      url('https://i.imgur.com/2ayEXRE.png') no-repeat left bottom,
      url('https://i.imgur.com/hE8e69N.png') no-repeat right bottom;
    background-size: 300px 150px, 250px 150px;
    opacity: 0.25;
    animation: sway 8s ease-in-out infinite alternate;
    z-index: 1;
  }
  @keyframes sway {
    0% { transform: translateX(0);}
    100% { transform: translateX(20px);}
  }
  /* Cabeçalho */
  header {
    position: relative;
    z-index: 2;
    text-align: center;
    padding: 50px 20px 30px 20px;
    background: rgba(0,0,0,0.7);
    border-bottom: 1px solid #444;
  }
  header h1 {
    font-size: 54px;
    color: #b22222;
    text-shadow: 2px 2px 6px #330000;
    font-weight: bold;
  }
  header p {
    font-size: 20px;
    color: #ccc;
    font-weight: 600;
    margin-top: 5px;
    letter-spacing: 2px;
  }
  /* Conteúdo */
  main {
    max-width: 900px;
    background: rgba(10,10,10,0.85);
    margin: 30px auto 60px auto;
    padding: 30px 25px 40px 25px;
    border-radius: 12px;
    box-shadow: 0 0 30px #440000cc;
    position: relative;
    z-index: 2;
  }
  h2 {
    color: #b22222;
    margin-bottom: 12px;
    border-bottom: 2px solid #550000;
    padding-bottom: 6px;
    font-weight: bold;
  }
  ul {
    list-style: none;
    margin-left: 10px;
    margin-bottom: 20px;
  }
  ul li {
    margin-bottom: 8px;
    line-height: 1.4;
    font-weight: 600;
  }
  /* Botão Discord */
  .btn-discord {
    display: inline-block;
    background: #7289da;
    color: white;
    padding: 14px 30px;
    font-weight: 700;
    font-size: 18px;
    border-radius: 7px;
    text-decoration: none;
    box-shadow: 0 0 15px #7289da88;
    transition: background-color 0.3s ease;
    margin-top: 15px;
  }
  .btn-discord:hover {
    background: #5b6eae;
  }
  /* Som ambiente - controle */
  #audioControl {
    position: fixed;
    bottom: 20px;
    right: 20px;
    z-index: 3;
  }
  #audioControl button {
    background: #b22222;
    border: none;
    color: #fff;
    font-size: 20px;
    padding: 10px 18px;
    border-radius: 50%;
    cursor: pointer;
    box-shadow: 0 0 10px #b2222288;
    transition: background 0.3s ease;
  }
  #audioControl button:hover {
    background: #7a1616;
  }
  /* Formulário */
  form {
    background: #220000dd;
    padding: 20px;
    border-radius: 10px;
  }
  form label {
    display: block;
    margin-bottom: 6px;
    font-weight: 700;
  }
  form input, form textarea {
    width: 100%;
    padding: 8px 12px;
    margin-bottom: 15px;
    border: none;
    border-radius: 5px;
    font-size: 16px;
  }
  form input[type="submit"] {
    background: #b22222;
    color: white;
    font-weight: 900;
    cursor: pointer;
    transition: background 0.3s ease;
    box-shadow: 0 0 15px #b2222288;
  }
  form input[type="submit"]:hover {
    background: #7a1616;
  }
  /* Mensagem sucesso */
  #msgSuccess {
    background: #228822bb;
    padding: 10px;
    border-radius: 6px;
    margin-top: 10px;
    font-weight: 700;
    display: none;
  }
  /* Responsivo simples */
  @media(max-width: 600px){
    header h1 { font-size: 36px; }
    header p { font-size: 14px;}
    main { margin: 20px 10px; padding: 20px 15px; }
  }
</style>
</head>
<body>

<div class="nebula"></div>
<div class="silhouettes"></div>

<header>
  <h1>☠️ SHADOW BORN ☠️</h1>
  <p>░▒▓【 CONVOCAÇÃO SOMBRIA — ⚫ SHADOW BORN 】▓▒░</p>
</header>

<main>
  <section>
    <h2>🔮 Você não está lendo isso por acaso...</h2>
    <p>A tripulação mais temida dos mares está chamando.
    Não somos uma crew qualquer. Somos uma lenda viva, forjada no nevoeiro, nas batalhas e no sangue dos antigos piratas.</p>
  </section>

  <section>
    <h2>🌊 EXPERIÊNCIAS QUE SÓ A SHADOW BORN OFERECE:</h2>
    <ul>
      <li>⚓ Eventos Marítimos Épicos – Navegue por mares tempestuosos em busca de glória.</li>
      <li>🏝️ Ilusões & Miragens Secretas – Descubra lugares que só os ousados alcançam.</li>
      <li>🌀 Ajuda Sempre Presente – Aqui, ninguém fica pra trás.</li>
      <li>🐉 Caça ao Leviathan – Enfrente monstros que testam até os mais fortes.</li>
      <li>🗡️ Torneios & PVP – Treinamentos intensos e combates por prestígio.</li>
      <li>🌕 Trials Sombrios e Exclusivos – Prove seu valor em desafios que moldam lendas.</li>
      <li>🔥 A Mítica Ilha do Vulcão – Apenas os destemidos sobrevivem.</li>
      <li>📰 Atualizações Frequentes – Sempre com novidades, melhorias e conteúdo insano.</li>
    </ul>
  </section>

  <section>
    <h2>🩸 NOSSA TRIPULAÇÃO TEM DIVISÕES DE ELITE:</h2>
    <ul>
      <li>👑 1ª Divisão – 20M+ | A Elite das Sombras</li>
      <li>⚓ 2ª Divisão – 10M a 20M | Comandantes do Caos</li>
      <li>⚔️ 3ª Divisão – 5M a 10M | Veteranos da Bruma</li>
      <li>🍃 4ª Divisão – 2.5M a 5M | Caçadores da Noite</li>
      <li>🐲 5ª Divisão – 0 a 2M | Novatos das Trevas</li>
    </ul>
  </section>

  <section>
    <h2>🕶️ POR QUE ESCOLHER A SHADOW BORN?</h2>
    <p>💀 Porque aqui… você não é apenas um nome.
    Você é parte de um legado.
    🌑 Você é o sopro frio da madrugada.
    Você é SHADOW.
    Você é BORN.
    E juntos… NÓS SOMOS TEMIDOS.</p>

    <a href="https://discord.gg/sE6MG8dg4W" class="btn-discord" target="_blank" rel="noopener">⛵ Entre na Shadow Born Agora</a>
  </section>

  <section>
    <h2>⚓ Alistamento dos Piratas</h2>
    <form id="formShadowBorn" action="#" onsubmit="return enviarEmail(event)">
      <label for="nome">Nome Completo</label>
      <input type="text" id="nome" name="nome" required placeholder="Seu nome verdadeiro" />

      <label for="nick">Nickname no Roblox</label>
      <input type="text" id="nick" name="nick" required placeholder="Seu apelido na crew" />

      <label for="discord">Link ou Nick do Discord</label>
      <input type="text" id="discord" name="discord" required placeholder="Seu Discord para contato" />

      <input type="submit" value="Enviar Alistamento" />
    </form>
    <div id="msgSuccess">⚓ Seu alistamento foi enviado! Verifique seu e-mail para confirmar.</div>
  </section>
</main>

<!-- Controle do som -->
<div id="audioControl">
  <button id="btnAudio" aria-label="Ligar/Desligar som ambiente">🔈</button>
</div>

<audio id="audio" loop>
  <source src="https://cdn.pixabay.com/download/audio/2021/11/22/audio_4db4b5f96f.mp3?filename=waves-at-sea-10054.mp3" type="audio/mpeg" />
  Seu navegador não suporta áudio.
</audio>

<script>
  // Som ambiente com botão ON/OFF
  const audio = document.getElementById('audio');
  const btnAudio = document.getElementById('btnAudio');
  let tocando = false;

  btnAudio.addEventListener('click', () => {
    if(tocando){
      audio.pause();
      btnAudio.textContent = '🔈';
      tocando = false;
    } else {
      audio.play();
      btnAudio.textContent = '🔊';
      tocando = true;
    }
  });

  // Enviar formulário 
    event.preventDefault();
    const nome = document.getElementById('nome').value.trim();
    const nick = document.getElementById('nick').value.trim();
    const discord = document.getElementById('discord').value.trim();

    if (!nome || !nick || !discord) {
      alert('Por favor, preencha todos os campos.');
      return false;
    }

    const email = 'seuemail@dominio.com'; // <<< Troque para seu e-mail aqui!
    const assunto = encodeURIComponent('Alistamento Shadow Born');
    const corpo = encodeURIComponent(
      `Nome Completo: ${nome}\nNickname no Roblox: ${nick}\nDiscord: ${discord}`
    );

    const mailtoLink = `mailto:${email}?subject=${assunto}&body=${corpo}`;
    window.location.href = mailtoLink;

    // Exibir mensagem (opcional)
    const msg = document.getElementById('msgSuccess');
    msg.style.display = 'block';

    // Resetar form
    document.getElementById('formShadowBorn').reset();

    return false;
  }
</script>

</body>
</html>
