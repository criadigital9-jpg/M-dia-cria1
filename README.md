/midia-cria
 ├─ index.html
 ├─ style.css
 └─ script.js<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Mídia Cria | Marketing & Design Digital</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Marketing digital, design gráfico, criação de sites, geração de leads e gestão de tráfego com Meta Ads.">
  <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="background"></div>

<header class="header">
  <div class="logo">MÍDIA <span>CRIA</span></div>
  <nav>
    <a href="#servicos">Serviços</a>
    <a href="#portfolio">Portfólio</a>
    <a href="#leads">Leads</a>
    <a href="#contato">Contato</a
  </nav>
</header>

<section class="hero">
  <h1>Transformamos ideias em <span>resultados digitais</span></h1>
  <p>Marketing digital estratégico, design profissional e tráfego pago para escalar sua marca.</p>
  <a href="#contato" class="btn">Quero Crescer Minha Marca</a>
</section>

<section id="servicos" class="section">
  <h2>Nossos Serviços</h2>
  <div class="cards">
    <div class="card">🎨 <h3>Design Digital</h3><p>Avatares, catálogos, cardápios, identidade visual e artes para redes sociais.</p></div>
    <div class="card">🌐 <h3>Criação de Sites</h3><p>Sites institucionais, páginas de vendas e landing pages focadas em conversão.</p></div>
    <div class="card">📈 <h3>Meta Ads</h3><p>Campanhas no Instagram e Facebook com segmentação estratégica.</p></div>
    <div class="card">🤝 <h3>Geração de Leads</h3><p>Estratégias para captar contatos qualificados e vender todos os dias.</p></div>
  </div>
</section>

<section id="portfolio" class="section dark">
  <h2>Portfólio</h2>
  <p>Alguns modelos de projetos desenvolvidos</p>
  <div class="portfolio">
    <div class="mockup">Avatar Profissional</div>
    <div class="mockup">Catálogo Digital</div>
    <div class="mockup">Cardápio Online</div>
    <div class="mockup">Landing Page</div>
    <div class="mockup">Anúncio Instagram</div>
    <div class="mockup">Identidade Visual</div>
  </div>
</section>

<section id="leads" class="section">
  <h2>Criação de Leads</h2>
  <p>Estrutura completa para atrair, capturar e converter clientes.</p>
  <ul class="leads">
    <li>✔ Páginas otimizadas</li>
    <li>✔ Anúncios estratégicos</li>
    <li>✔ Copy persuasiva</li>
    <li>✔ Automação de contatos</li>
  </ul>
</section>

<section id="contato" class="section dark">
  <h2>Vamos criar seu próximo projeto?</h2>
  <p>Entre em contato e transforme sua presença digital.</p>
  <a class="btn" href="https://wa.me/5521979058213" target="_blank">Falar no WhatsApp</a>
</section>

<footer>
  <p>© 2025 Mídia Cria — Marketing & Design Digital</p>
</footer>

<script src="script.js"></script>
</body>
</html>* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  color: #222;
  overflow-x: hidden;
}

.background {
  position: fixed;
  width: 100%;
  height: 100%;
  background: linear-gradient(120deg, #e0f7ff, #f5e9ff);
  animation: gradient 10s infinite alternate;
  z-index: -1;
}

@keyframes gradient {
  0% { filter: hue-rotate(0deg); }
  100% { filter: hue-rotate(40deg); }
}

.header {
  display: flex;
  justify-content: space-between;
  padding: 20px 60px;
  position: sticky;
  top: 0;
  backdrop-filter: blur(10px);
}

.logo {
  font-size: 26px;
  font-weight: bold;
}

.logo span {
  color: #7a00ff;
}

nav a {
  margin-left: 20px;
  text-decoration: none;
  color: #222;
  font-weight: 500;
}

.hero {
  text-align: center;
  padding: 120px 20px;
}

.hero h1 {
  font-size: 48px;
}

.hero span {
  color: #7a00ff;
}

.btn {
  display: inline-block;
  margin-top: 30px;
  padding: 15px 35px;
  background: #7a00ff;
  color: white;
  border-radius: 30px;
  text-decoration: none;
}

.section {
  padding: 80px 60px;
  text-align: center;
}

.section.dark {
  background: rgba(0,0,0,0.05);
}

.cards, .portfolio {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px,1fr));
  gap: 25px;
  margin-top: 40px;
}

.card, .mockup {
  padding: 30px;
  border-radius: 15px;
  background: white;
  box-shadow: 0 10px 30px rgba(0,0,0,0.08);
}

.leads {
  list-style: none;
  margin-top: 30px;
  font-size: 18px;
}

footer {
  padding: 30px;
  text-align: center;
}// Interação simples de entrada
const elements = document.querySelectorAll('.card, .mockup');

elements.forEach(el => {
  el.addEventListener('mouseenter', () => {
    el.style.transform = 'scale(1.05)';
  });
  el.addEventListener('mouseleave', () => {
    el.style.transform = 'scale(1)';
  });
});<section id="portfolio" class="section dark">
  <h2>Portfólio</h2>
  <p>Projetos desenvolvidos para marcas que buscam resultado</p>

  <div class="portfolio">
    <div class="portfolio-item">
      <img src="https://images.unsplash.com/photo-1559028012-481c04fa702d" alt="Avatar profissional">
      <div class="overlay">
        <h3>Avatar Profissional</h3>
        <a href="https://wa.me/5521979058213" target="_blank">Solicitar Projeto</a>
      </div>
    </div>

    <div class="portfolio-item">
      <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f" alt="Catálogo digital">
      <div class="overlay">
        <h3>Catálogo Digital</h3>
        <a href="https://wa.me/5521979058213" target="_blank">Solicitar Projeto</a>
      </div>
    </div>

    <div class="portfolio-item">
      <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836" alt="Cardápio digital">
      <div class="overlay">
        <h3>Cardápio Online</h3>
        <a href="https://wa.me/5521979058213" target="_blank">Solicitar Projeto</a>
      </div>
    </div>

    <div class="portfolio-item">
      <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085" alt="Site profissional">
      <div class="overlay">
        <h3>Criação de Sites</h3>
        <a href="https://wa.me/5521979058213" target="_blank">Solicitar Projeto</a>
      </div>
    </div>

    <div class="portfolio-item">
      <img src="https://images.unsplash.com/photo-1557838923-2985c318be48" alt="Meta Ads">
      <div class="overlay">
        <h3>Meta Ads</h3>
        <a href="https://wa.me/5521979058213" target="_blank">Criar Anúncio</a>
      </div>
    </div>

    <div class="portfolio-item">
      <img src="https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7" alt="Instagram">
      <div class="overlay">
        <h3>Impulsionamento Instagram</h3>
        <a href="https://wa.me/5521979058213" target="_blank">Impulsionar</a>
      </div>
    </div>
  </div>
</section>.portfolio-item {
  position: relative;
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 15px 40px rgba(0,0,0,0.15);
}

.portfolio-item img {
  width: 100%;
  height: 260px;
  object-fit: cover;
  transition: transform 0.4s;
}

.portfolio-item:hover img {
  transform: scale(1.1);
}

.overlay {
  position: absolute;
  inset: 0;
  background: rgba(0,0,0,0.65);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  opacity: 0;
  transition: 0.4s;
  color: white;
}

.portfolio-item:hover .overlay {
  opacity: 1;
}

.overlay a {
  margin-top: 10px;
  padding: 10px 25px;
  background: #7a00ff;
  color: white;
  border-radius: 25px;
  text-decoration: none;
}<a href="https://wa.me/5521979058213" class="whatsapp-float" target="_blank">
  💬
</a>.whatsapp-float {
  position: fixed;
  bottom: 25px;
  right: 25px;
  width: 60px;
  height: 60px;
  background: #25d366;
  color: white;
  font-size: 28px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  box-shadow: 0 10px 25px rgba(0,0,0,0.3);
  z-index: 999;
}
