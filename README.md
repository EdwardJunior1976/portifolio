<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Portfólio - Edward Ferreira Junior</title>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body { font-family: 'Roboto', sans-serif; background: #f4f4f9; color: #333; scroll-behavior: smooth; }
  header { background: linear-gradient(135deg, #3b82f6, #1e40af); color: #fff; text-align: center; padding: 2rem 1rem; }
  header h1 { font-size: 2.5rem; margin-bottom: 0.5rem; }
  header p { font-size: 1.1rem; margin-bottom: 0.3rem; }
  nav { background: #1e40af; text-align: center; padding: 0.5rem; position: sticky; top: 0; z-index: 100; }
  nav a { color: #fff; margin: 0 1rem; text-decoration: none; font-weight: 500; transition: 0.3s; }
  nav a:hover { text-decoration: underline; }
  section { max-width: 900px; margin: 2rem auto; padding: 2rem; background: #fff; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); opacity: 0; transform: translateY(50px); transition: all 0.8s ease; }
  section.visible { opacity: 1; transform: translateY(0); }
  section h2 { color: #1e40af; border-bottom: 3px solid #3b82f6; padding-bottom: 0.5rem; margin-bottom: 1rem; }
  ul { list-style-type: disc; padding-left: 1.5rem; margin-top: 0.5rem; }
  .experience-item { margin-bottom: 1rem; border-bottom: 1px solid #ddd; }
  .experience-item button { background: none; border: none; width: 100%; text-align: left; font-size: 1.1rem; font-weight: 700; padding: 0.5rem 0; cursor: pointer; color: #1e40af; }
  .experience-item button:hover { color: #3b82f6; }
  .experience-content { display: none; padding: 0.5rem 1rem; }
  footer { text-align: center; padding: 1rem; background: #1e40af; color: #fff; margin-top: 2rem; }
  footer a { color: #3b82f6; text-decoration: none; }
  footer a:hover { text-decoration: underline; }
  .buttons { text-align: center; margin: 1rem 0; }
  .buttons a { background: #3b82f6; color: #fff; padding: 0.6rem 1.2rem; border-radius: 5px; margin: 0 0.5rem; text-decoration: none; font-weight: 500; transition: 0.3s; }
  .buttons a:hover { background: #1e40af; }
  .chart-container { max-width: 600px; margin: 1rem auto; }
</style>
</head>
<body>

<header>
  <h1>Edward Ferreira Junior</h1>
  <p>Analista de Negócios e Requisitos | Metodologias Ágeis e Transformação Digital</p>
  <p>Email: <a href="mailto:edwardjunior30@gmail.com">edwardjunior30@gmail.com</a> | Contato: (65) 9 9203-8202 | Cuiabá-MT</p>
  <div class="buttons">
    <a href="#" onclick="alert('PDF do currículo será baixado!');">📄 Baixar Currículo</a>
    <a href="https://www.linkedin.com/in/ferreiraedward/" target="_blank">LinkedIn</a>
    <a href="#" target="_blank">GitHub</a>
    <a href="#" target="_blank">Portfólio de Protótipos</a>
  </div>
</header>

<nav>
  <a href="#resumo">Resumo</a>
  <a href="#formacao">Formação</a>
  <a href="#conquistas">Conquistas</a>
  <a href="#habilidades">Habilidades</a>
  <a href="#experiencia">Experiência</a>
  <a href="#skillschart">Skills</a>
</nav>

<section id="resumo">
  <h2>Resumo Profissional</h2>
  <p>Analista de Negócios e Requisitos com sólida experiência em órgãos públicos e empresas privadas. Atuação em levantamento, análise e documentação de requisitos, desenho de processos de negócio, apoio a áreas de produto e design, pesquisa com usuários e definição de soluções digitais. Experiência como PMO e Analista de Suporte Técnico, visão completa do ciclo de vida de projetos.</p>
</section>

<section id="formacao">
  <h2>Formação Acadêmica</h2>
  <ul>
    <li><strong>MBA Executivo em Gestão de Projetos (PMI-PMBOK)</strong> – Facuminas (02/2022 – 10/2024)</li>
    <li><strong>Bacharel em Ciências da Computação</strong> – UNORP (01/1999 – 12/2003)</li>
  </ul>
</section>

<section id="conquistas">
  <h2>Principais Conquistas</h2>
  <ul>
    <li>Transformação Digital: +25% de eficiência operacional</li>
    <li>Otimização de Processos: -50% de erros manuais, +40% produtividade</li>
    <li>Redução de Custos: -20% despesas operacionais</li>
    <li>Gestão de Equipes: Liderança de times de até 15 pessoas</li>
    <li>Gestão de Stakeholders: Alinhamento de expectativas entre equipes técnicas e gestores</li>
  </ul>
</section>

<section id="habilidades">
  <h2>Habilidades e Especializações</h2>
  <ul>
    <li>Metodologias Ágeis: Scrum, Kanban, facilitação de cerimônias</li>
    <li>ServiceNow: ITSM, ITOM, HRSD, CSM</li>
    <li>Gestão de Requisitos: Ferramentas RDNG, modelagem formal, documentação completa</li>
    <li>Análise de Negócios e Produtos: Levantamento de processos, análise de MVP, validação com usuários</li>
    <li>Métricas e Avaliação: Análise de Ponto de Função (APF)</li>
  </ul>
</section>

<section id="skillschart">
  <h2>Skills e KPIs</h2>
  <div class="chart-container">
    <canvas id="skillsChart"></canvas>
  </div>
</section>

<section id="experiencia">
  <h2>Experiência Profissional</h2>

  <div class="experience-item">
    <button>Qintess – Analista de Negócios e Requisitos (Projeto TJBA) <em>(04/2025 – 08/2025)</em></button>
    <div class="experience-content">
      <ul>
        <li>Definição e documentação de processos de negócios e requisitos</li>
        <li>Suporte a times de design e produto</li>
        <li>Condução de pesquisas de usuários e desenvolvimento de conceitos</li>
        <li>Planejamento, execução e consolidação de pesquisas qualitativas</li>
      </ul>
    </div>
  </div>

  <div class="experience-item">
    <button>Softplan – Analista de Serviço Pessoal II (Ministério Público) <em>(08/2022 – 09/2023)</em></button>
    <div class="experience-content">
      <ul>
        <li>Liderança de projetos complexos: +25% eficiência, -20% custos</li>
        <li>Coordenação de parametrizações, configurações, homologações e treinamentos</li>
        <li>Comunicação com stakeholders e relatórios estratégicos</li>
        <li>Conquistas: +50% conformidade, -20% incidentes críticos</li>
      </ul>
    </div>
  </div>

  <div class="experience-item">
    <button>SuporTI Digital – Consultor de Suporte Técnico <em>(01/2020 – 01/2022)</em></button>
    <div class="experience-content">
      <ul>
        <li>Resolução de incidentes técnicos e otimização de rotinas</li>
        <li>Elaboração de propostas técnicas e comerciais</li>
        <li>Conquistas: +40% eficiência, -50% erros manuais</li>
      </ul>
    </div>
  </div>

  <div class="experience-item">
    <button>Ilha Service – Supervisor Service Desk <em>(05/2021 – 01/2022)</em></button>
    <div class="experience-content">
      <ul>
        <li>Gestão de demandas e tickets de atendimento</li>
        <li>Liderança de equipe multidisciplinar (15 pessoas)</li>
        <li>Conquistas: -30% tempo inatividade, +25% satisfação, +30% velocidade resolução, -75% reclamações</li>
      </ul>
    </div>
  </div>

  <div class="experience-item">
    <button>Grupo Tecnowise / Prosimulador – Analista de Negócio e Suporte <em>(12/2018 – 12/2019)</em></button>
    <div class="experience-content">
      <ul>
        <li>Condução de workshops, levantamento de requisitos e definição de escopo</li>
        <li>Treinamento e suporte a usuários finais</li>
        <li>Conquistas: -35% tempo treinamento, +40% produtividade</li>
      </ul>
    </div>
  </div>

</section>

<footer>
  <p>© 2025 Edward Ferreira Junior | <a href="mailto:edwardjunior30@gmail.com">edwardjunior30@gmail.com</a></p>
</footer>

<script>
  // Animação ao rolar
  const sections = document.querySelectorAll('section');
  window.addEventListener('scroll', () => {
    sections.forEach(section => {
      const top = section.getBoundingClientRect().top;
      const windowHeight = window.innerHeight;
      if(top < windowHeight - 100) section.classList.add('visible');
    });
  });

  // Toggle experiência
  document.querySelectorAll('.experience-item button').forEach(btn => {
    btn.addEventListener('click', () => {
      const content = btn.nextElementSibling;
      content.style.display = content.style.display === 'block' ? 'none' : 'block';
    });
  });

  // Chart.js Skills
  const ctx = document.getElementById('skillsChart').getContext('2d');
  const skillsChart = new Chart(ctx, {
    type: 'bar',
    data: {
      labels: ['Análise de Negócios', 'Gestão de Projetos', 'Metodologias Ágeis', 'ServiceNow', 'Comunicação', 'Documentação'],
      datasets: [{
        label: 'Nível de Habilidade (%)',
        data: [95, 90, 85, 80, 90, 95],
        backgroundColor: '#3b82f6'
      }]
    },
    options: {
      responsive: true,
      scales: { y: { beginAtZero: true, max: 100 } }
    }
  });
</script>

</body>
</html>
