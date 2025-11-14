---
title: "Meus Projetos"
layout: single
permalink: /portfolio/
classes: wide
author_profile: false
---

<style>
/* ====================MUDANÇA FEITA ==================== */

/* Customizações só para /portfolio/ */
.page--portfolio {
  .page__content {
    margin-left: auto;
    margin-right: auto;
    max-width: 1100px;
    padding-left: 20px;
    padding-right: 20px;
    box-sizing: border-box;
  }

  /* Centraliza o hero text se existir */
  .custom-hero-text {
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }

  .project-buttons {
    display: flex;
    flex-direction: column; /* empilha verticalmente */
    gap: 10px;
    align-items: center;
  }

  .btn-custom {
    width: 100%;
    max-width: 240px;
    text-align: center;
  }
}

/* ==================== TÍTULO PRINCIPAL ==================== */
.page__title {
  text-align: center;
  font-size: 48px !important;
  color: #ffffff !important;
  margin-bottom: 20px !important;
  text-shadow: 2px 2px 10px rgba(77, 166, 255, 0.5);
  background: linear-gradient(90deg, #4da6ff, #00ccff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* ==================== SUBTÍTULO ==================== */
.intro-text {
  text-align: center;
  font-size: 20px;
  color: #cccccc;
  margin-bottom: 50px;
  max-width: 800px;
  margin-left: auto;
  margin-right: auto;
}

/* ==================== GRID DE PROJETOS ==================== */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 30px;
  margin: 40px auto;
  padding: 0 15px;
  width: 100%;
  box-sizing: border-box;
}

/* ==================== CARD DE PROJETO ==================== */
.project-card {
  width: 100%;
  box-sizing: border-box;
  background: linear-gradient(145deg, rgba(20, 40, 80, 0.8), rgba(10, 20, 40, 0.9));
  border: 2px solid transparent;
  border-radius: 15px;
  padding: 30px;
  transition: all 0.4s ease;
  position: relative;
  overflow: hidden;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.5);
}

/* ==================== BOTÕES ==================== */
.project-buttons {
  display: flex;
  flex-direction: column; /* empilha verticalmente */
  gap: 10px;
  justify-content: center;
  align-items: center;
  margin-top: 25px;
}

/* Ordem: GitHub primeiro, depois Documentação */
.btn-github {
  background: linear-gradient(135deg, #333333, #1a1a1a);
  color: #ffffff;
  border-color: #333333;
}

.btn-github:hover {
  background: linear-gradient(135deg, #4da6ff, #0088cc);
  border-color: #4da6ff;
  transform: translateY(-2px);
  box-shadow: 0 5px 20px rgba(77, 166, 255, 0.4);
}

.btn-demo {
  background: transparent;
  color: #4da6ff;
  border-color: #4da6ff;
}

.btn-demo:hover {
  background: rgba(77, 166, 255, 0.1);
  transform: translateY(-2px);
}

/* ==================== RESPONSIVO ==================== */
@media (max-width: 768px) {
  .projects-grid {
    grid-template-columns: 1fr;
    gap: 25px;
    padding: 0 15px;
  }
  
  .page__title {
    font-size: 36px !important;
  }
  
  .intro-text {
    font-size: 18px;
  }
  
  .project-card {
    padding: 25px;
  }
  
  .project-buttons {
    flex-direction: column;
  }
  
  .btn-custom {
    width: 100%;
    justify-content: center;
  }
}
</style>


<!-- Introdução -->
<p class="intro-text">
  🚀 Confira alguns dos meus projetos mais relevantes em <strong>infraestrutura, redes e automação</strong>. Cada projeto foi desenvolvido com foco em eficiência, automação e boas práticas de desenvolvimento.
</p>

<!-- Grid de Projetos -->
<div class="projects-grid">

  <!-- Projeto 1: Modem VIVO Unlock -->
  <div class="project-card">
    <span class="status-badge">✓ Ativo</span>
    
    <div class="project-icon">
      📡
    </div>
    
    <h2 class="project-title">Modem VIVO Unlock</h2>
    
    <p class="project-description">
      Ferramenta de automação completa para desbloqueio de configurações avançadas do modem Askey RTF8115VW REV5 (VIVO). Desenvolvida com Node.js e Selenium WebDriver para automatizar o processo de forma segura e eficiente.
    </p>
    
    <div class="tech-tags">
      <span class="tech-tag">Node.js</span>
      <span class="tech-tag">Selenium</span>
      <span class="tech-tag">PowerShell</span>
      <span class="tech-tag">ChromeDriver</span>
      <span class="tech-tag">JavaScript</span>
    </div>
    
    <div class="project-buttons">
      <a href="https://github.com/edgardocorrea/modem-vivo" class="btn-custom btn-github" target="_blank">
        <i class="fab fa-github"></i> Ver no GitHub
      </a>
      <a href="https://github.com/edgardocorrea/modem-vivo#readme" class="btn-custom btn-demo" target="_blank">
        <i class="fas fa-book"></i> Documentação
      </a>
    </div>
  </div>

  <!-- Projeto 2: Limpeza Avançada Windows -->
  <div class="project-card">
    <span class="status-badge">✓ Ativo</span>
    
    <div class="project-icon">
      🧹
    </div>
    
    <h2 class="project-title">Limpeza Avançada Windows</h2>
    
    <p class="project-description">
      Script PowerShell automatizado para limpeza profunda do Windows. Remove arquivos temporários, cache, logs e otimiza o sistema operacional com interface intuitiva e opções avançadas de personalização.
    </p>
    
    <div class="tech-tags">
      <span class="tech-tag">PowerShell</span>
      <span class="tech-tag">Windows API</span>
      <span class="tech-tag">Batch</span>
      <span class="tech-tag">Automação</span>
    </div>
    
    <div class="project-buttons">
      <a href="https://github.com/edgardocorrea/LimpezaAvancada" class="btn-custom btn-github" target="_blank">
        <i class="fab fa-github"></i> Ver no GitHub
      </a>
      <a href="https://github.com/edgardocorrea/LimpezaAvancada#readme" class="btn-custom btn-demo" target="_blank">
        <i class="fas fa-book"></i> Documentação
      </a>
    </div>
  </div>

  <!-- Projeto 3: (Adicione mais projetos aqui) -->
  <div class="project-card">
    <span class="status-badge" style="background: linear-gradient(135deg, #ffcc00, #ff9900);">⏳ Em Breve</span>
    
    <div class="project-icon">
      🔧
    </div>
    
    <h2 class="project-title">Outros Projetos</h2>
    
    <p class="project-description">
      Novos projetos de infraestrutura, automação e desenvolvimento em andamento. Fique atento para mais atualizações em breve!
    </p>
    
    <div class="tech-tags">
      <span class="tech-tag">Em Desenvolvimento</span>
    </div>
    
    <div class="project-buttons">
      <a href="https://github.com/edgardocorrea" class="btn-custom btn-github" target="_blank">
        <i class="fab fa-github"></i> Ver GitHub
      </a>
    </div>
  </div>

</div>

