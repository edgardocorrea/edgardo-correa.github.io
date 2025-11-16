---
layout: single
title: "Sobre Mim"
permalink: /sobre/
author_profile: false
---

<style>
/* ==================== RESET & BASE (ISOLADO) ==================== */
/* ALTERADO: O reset agora afeta apenas o nosso wrapper, não o site inteiro. */
#custom-sobre-page,
#custom-sobre-page * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* ALTERADO: O 'body' para esta página é agora o nosso wrapper. */
#custom-sobre-page {
  font-family: 'Inter', 'Segoe UI', sans-serif;
  overflow-x: hidden; /* Previne rolagem horizontal */
  position: relative; /* Contexto para os elementos posicionados */
  background-color: #000814; /* Fundo para a página inteira */
  color: #ffffff;
}

/* O .initial-content é do tema, vamos apenas garantir que ele não atrapalhe */
.initial-content {
  position: relative;
  background: transparent; /* Deixa o fundo do nosso wrapper aparecer */
  padding: 0 !important; /* Remove o padding do tema */
  border-radius: 0 !important; /* Remove a borda do tema */
  box-shadow: none !important; /* Remove a sombra do tema */
  max-width: 100% !important; /* Ocupa toda a largura disponível */
}

/* ==================== PARTÍCULAS DE FUNDO ==================== */
/* Sem mudanças necessárias aqui, mas vamos isolar por segurança */
#custom-sobre-page .particles-bg {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
  pointer-events: none;
  background: radial-gradient(circle at 20% 30%, rgba(0, 234, 255, 0.03) 0%, transparent 50%), radial-gradient(circle at 80% 70%, rgba(0, 102, 255, 0.03) 0%, transparent 50%);
}
#custom-sobre-page .particles-bg::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  background-image: repeating-linear-gradient(0deg, rgba(0, 234, 255, 0.03) 0px, transparent 2px, transparent 40px), repeating-linear-gradient(90deg, rgba(0, 234, 255, 0.03) 0px, transparent 2px, transparent 40px);
  animation: gridMove 20s linear infinite;
}
@keyframes gridMove { /* ... */ }

/* ==================== HERO SECTION ==================== */
/* ALTERADO: Removido o min-height conflitante. Agora usa padding para preencher a tela. */
#custom-sobre-page .hero-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  /* Ajuste estes valores conforme necessário para preencher a tela verticalmente */
  padding: 120px 20px 80px 20px; 
  min-height: 90vh; /* Uma abordagem mais segura que 100vh */
  z-index: 1;
}

/* ... O restante dos seus estilos para .sobre-brilhante, .avatar-container, etc. devem ser prefixados ... */
#custom-sobre-page .sobre-brilhante { /* ... */ }
#custom-sobre-page .avatar-container { /* ... */ }
#custom-sobre-page .avatar-glow { /* ... */ }
#custom-sobre-page .avatar-container img { /* ... */ }
@keyframes float { /* ... */ }
@keyframes pulse { /* ... */ }
#custom-sobre-page .hero-title { /* ... */ }
@keyframes gradient { /* ... */ }
#custom-sobre-page .typewriter { /* ... */ }
@keyframes typing { /* ... */ }
@keyframes blink { /* ... */ }
#custom-sobre-page .hero-description { /* ... */ }
#custom-sobre-page .cta-button { /* ... */ }
#custom-sobre-page .cta-button:hover { /* ... */ }
@keyframes ctaPulse { /* ... */ }
#custom-sobre-page .scroll-indicator { /* ... */ }
@keyframes bounce { /* ... */ }

/* ==================== SEÇÕES EXPANSÍVEIS ==================== */
#custom-sobre-page .content-section {
  position: relative;
  z-index: 1;
  padding: 0 20px 80px 20px; /* Adiciona padding na parte de baixo */
}
#custom-sobre-page .section-accordion { /* ... */ }
#custom-sobre-page .section-accordion:hover { /* ... */ }
#custom-sobre-page .accordion-header { /* ... */ }
#custom-sobre-page .accordion-title { /* ... */ }
#custom-sobre-page .accordion-icon { /* ... */ }
#custom-sobre-page .accordion-header:hover .accordion-icon { /* ... */ }
#custom-sobre-page .accordion-arrow { /* ... */ }
#custom-sobre-page .section-accordion.active .accordion-arrow { /* ... */ }
#custom-sobre-page .accordion-content { /* ... */ }
#custom-sobre-page .section-accordion.active .accordion-content { /* ... */ }

/* ... Continue prefixando TODOS os outros seletores ... */
/* Exemplo: */
/* .timeline vira #custom-sobre-page .timeline */
/* .skills-grid vira #custom-sobre-page .skills-grid */
/* E assim por diante... */

/* ==================== RESPONSIVO ==================== */
@media (max-width: 768px) {
  #custom-sobre-page .hero-title { font-size: 42px; }
  #custom-sobre-page .typewriter { font-size: 20px; }
  #custom-sobre-page .hero-description { font-size: 16px; }
  #custom-sobre-page .timeline::before { left: 20px; }
  #custom-sobre-page .timeline-item { flex-direction: column !important; margin-left: 40px; }
  #custom-sobre-page .timeline-content { width: 100%; }
  #custom-sobre-page .timeline-dot { left: 20px; }
  #custom-sobre-page .accordion-title { font-size: 22px; }
  #custom-sobre-page .skills-grid { grid-template-columns: 1fr; }
}
</style>



<!-- Partículas de Fundo -->
<div class="particles-bg"></div>

<!-- Hero Section -->
<section class="hero-section">
  <div class="avatar-container">
    <div class="avatar-glow"></div>
    <img src="/assets/images/minha_foto.png" alt="Logo EC" />
  </div>
  
  <h1 class="hero-title">EDGARDO CORREA</h1>
  
  <div class="typewriter">Analista de Sistemas</div>
  
  <p class="hero-description">
    Transformando desafios técnicos em soluções elegantes. 
    Especializado em infraestrutura, redes e automação com paixão por inovação.
  </p>
  
  <a href="#contato" class="cta-button">Entre em contato comigo.</a>
  
  <div class="scroll-indicator">
    <span style="font-size: 32px;">↓</span>
  </div>
</section>

<!-- Conteúdo Principal -->
<div class="content-section">

  <!-- Sobre Mim -->
  <div class="section-accordion">
    <div class="accordion-header" onclick="toggleAccordion(this)">
      <div class="accordion-title">
        <span class="accordion-icon">🔷</span>
        <span class="sobre-brilhante">Sobre Mim</span>
      </div>
      <span class="accordion-arrow">▼</span>
    </div>
    <div class="accordion-content">
      <p style="color: #b3d9ff; line-height: 1.8; font-size: 16px;">
        Formado em <strong style="color: #00eaff;">Sistemas de Informação</strong> e movido pela paixão em resolver problemas complexos de forma criativa. Acredito que tecnologia é sobre pessoas — criar soluções que realmente fazem diferença no dia a dia.
      </p>
      <p style="color: #b3d9ff; line-height: 1.8; font-size: 16px; margin-top: 15px;">
        Minha filosofia: <strong style="color: #00ff88;">"Todo problema tem solução, e cada desafio é uma oportunidade de crescimento."</strong> Adoro trabalhar em equipe, compartilhar conhecimento e trazer energia positiva para os projetos.
      </p>
      <p style="color: #b3d9ff; line-height: 1.8; font-size: 16px; margin-top: 15px;">
        Quando não estou codando ou resolvendo tickets, você me encontra assistindo animes, explorando novas tecnologias ou pensando em como automatizar processos do dia a dia. 
      </p>
    </div>
  </div>

  <!-- Habilidades -->
  <div class="section-accordion">
    <div class="accordion-header" onclick="toggleAccordion(this)">
      <div class="accordion-title">
        <span class="accordion-icon">🔷</span>
        <span>Arsenal Técnico</span>
      </div>
      <span class="accordion-arrow">▼</span>
    </div>
    <div class="accordion-content">
      <div class="skills-grid">
        <div>
          <h3 style="color: #00eaff; margin-bottom: 20px;">Infraestrutura & Redes</h3>
          
          <div class="skill-item">
            <div class="skill-header">
              <span class="skill-name">Windows Server</span>
              <span class="skill-level">90%</span>
            </div>
            <div class="skill-bar">
              <div class="skill-fill" style="--skill-width: 90%;"></div>
            </div>
          </div>
          
          <div class="skill-item">
            <div class="skill-header">
              <span class="skill-name">Active Directory</span>
              <span class="skill-level">85%</span>
            </div>
            <div class="skill-bar">
              <div class="skill-fill" style="--skill-width: 85%;"></div>
            </div>
          </div>
          
          <div class="skill-item">
            <div class="skill-header">
              <span class="skill-name">Redes & VPN</span>
              <span class="skill-level">80%</span>
            </div>
            <div class="skill-bar">
              <div class="skill-fill" style="--skill-width: 80%;"></div>
            </div>
          </div>
        </div>
        
        <div>
          <h3 style="color: #00eaff; margin-bottom: 20px;">Automação & Desenvolvimento</h3>
          
          <div class="skill-item">
            <div class="skill-header">
              <span class="skill-name">PowerShell</span>
              <span class="skill-level">85%</span>
            </div>
            <div class="skill-bar">
              <div class="skill-fill" style="--skill-width: 85%;"></div>
            </div>
          </div>
          
          <div class="skill-item">
            <div class="skill-header">
              <span class="skill-name">Node.js</span>
              <span class="skill-level">75%</span>
            </div>
            <div class="skill-bar">
              <div class="skill-fill" style="--skill-width: 75%;"></div>
            </div>
          </div>
          
          <div class="skill-item">
            <div class="skill-header">
              <span class="skill-name">JavaScript</span>
              <span class="skill-level">80%</span>
            </div>
            <div class="skill-bar">
              <div class="skill-fill" style="--skill-width: 80%;"></div>
            </div>
          </div>
        </div>
      </div>
      
      <h3 style="color: #00eaff; margin-top: 40px; margin-bottom: 20px;">Soft Skills</h3>
      <div style="display: flex; flex-wrap: wrap; gap: 10px;">
        <span style="background: rgba(0, 234, 255, 0.2); border: 1px solid #00eaff; color: #00eaff; padding: 8px 16px; border-radius: 20px;">🤝 Trabalho em Equipe</span>
        <span style="background: rgba(0, 234, 255, 0.2); border: 1px solid #00eaff; color: #00eaff; padding: 8px 16px; border-radius: 20px;">💬 Comunicação Clara</span>
        <span style="background: rgba(0, 234, 255, 0.2); border: 1px solid #00eaff; color: #00eaff; padding: 8px 16px; border-radius: 20px;">🎯 Foco em Resultados</span>
        <span style="background: rgba(0, 234, 255, 0.2); border: 1px solid #00eaff; color: #00eaff; padding: 8px 16px; border-radius: 20px;">🚀 Proatividade</span>
        <span style="background: rgba(0, 234, 255, 0.2); border: 1px solid #00eaff; color: #00eaff; padding: 8px 16px; border-radius: 20px;">😊 Otimismo</span>
        <span style="background: rgba(0, 234, 255, 0.2); border: 1px solid #00eaff; color: #00eaff; padding: 8px 16px; border-radius: 20px;">📚 Aprendizado Contínuo</span>
      </div>
    </div>
  </div>

  <!-- Interesses -->
  <div class="section-accordion">
    <div class="accordion-header" onclick="toggleAccordion(this)">
      <div class="accordion-title">
        <span class="accordion-icon">🔷</span>
        <span>Além do Código</span>
      </div>
      <span class="accordion-arrow">▼</span>
    </div>
    <div class="accordion-content">
      <div class="interests-grid">
        <div class="interest-card">
          <span class="interest-icon">🔹</span>
          <div class="interest-title">Animes & Séries</div>
        </div>
        <div class="interest-card">
          <span class="interest-icon">🔹</span>
          <div class="interest-title">Inteligência Artificial</div>
        </div>
        <div class="interest-card">
          <span class="interest-icon">🔹</span>
          <div class="interest-title">Automação</div>
        </div>
        <div class="interest-card">
          <span class="interest-icon">🔹</span>
          <div class="interest-title">Inovação Tech</div>
        </div>
        <div class="interest-card">
          <span class="interest-icon">🔹</span>
          <div class="interest-title">Podcasts Tech</div>
        </div>
        <div class="interest-card">
          <span class="interest-icon">🔹</span>
          <div class="interest-title">Web Development</div>
        </div>
      </div>
    </div>
  </div>

  <!-- Contato -->
  <div class="section-accordion" id="contato">
    <div class="accordion-header" onclick="toggleAccordion(this)">
      <div class="accordion-title">
        <span class="accordion-icon">🔷</span>
        <span>Vamos Conectar?</span>
      </div>
      <span class="accordion-arrow">▼</span>
    </div>
    <div class="accordion-content">
      <p style="color: #b3d9ff; text-align: center; margin-bottom: 30px; font-size: 18px;">
        Sempre aberto para conversas sobre tecnologia, oportunidades ou apenas trocar ideias! 🚀
      </p>
      
      <div class="social-links">
        <a href="https://linkedin.com/in/edgardocorrea" class="social-card linkedin" target="_blank">
          <span class="social-icon">💼</span>
          <div class="social-title">LinkedIn</div>
          <div class="social-description">Conecte-se profissionalmente</div>
        </a>
        
        <a href="https://github.com/edgardocorrea" class="social-card github" target="_blank">
          <span class="social-icon">💻</span>
          <div class="social-title">GitHub</div>
          <div class="social-description">Explore meus projetos</div>
        </a>
        
        <a href="mailto:seu-email@exemplo.com" class="social-card email">
          <span class="social-icon">📧</span>
          <div class="social-title">Email</div>
          <div class="social-description">Envie uma mensagem direta</div>
        </a>
      </div>
    </div>
  </div>

</div>

<!-- Script para Acordeão -->
<script>
function toggleAccordion(header) {
  const accordion = header.parentElement;
  const allAccordions = document.querySelectorAll('.section-accordion');
  
  // Fecha todos os outros acordeões
  allAccordions.forEach(acc => {
    if (acc !== accordion && acc.classList.contains('active')) {
      acc.classList.remove('active');
    }
  });
  
  // Toggle do acordeão clicado
  accordion.classList.toggle('active');
  
  // Smooth scroll para o acordeão
  if (accordion.classList.contains('active')) {
    setTimeout(() => {
      accordion.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
    }, 100);
  }
}

// Animação das skills quando a seção é aberta
document.querySelectorAll('.section-accordion').forEach(accordion => {
  accordion.addEventListener('transitionend', function(e) {
    if (e.propertyName === 'max-height' && this.classList.contains('active')) {
      const skills = this.querySelectorAll('.skill-fill');
      skills.forEach((skill, index) => {
        setTimeout(() => {
          skill.style.width = skill.style.getPropertyValue('--skill-width');
        }, index * 100);
      });
    }
  });
});

// Smooth scroll para âncoras
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function (e) {
    e.preventDefault();
    const target = document.querySelector(this.getAttribute('href'));
    if (target) {
      target.scrollIntoView({ behavior: 'smooth', block: 'start' });
      
      // Abre o acordeão se for um link para seção
      const accordion = target.closest('.section-accordion');
      if (accordion && !accordion.classList.contains('active')) {
        accordion.querySelector('.accordion-header').click();
      }
    }
  });
});

// Efeito de typewriter no hero
const typewriterText = document.querySelector('.typewriter');
if (typewriterText) {
  const text = typewriterText.textContent;
  typewriterText.textContent = '';
  typewriterText.style.width = '0';
  
  setTimeout(() => {
    typewriterText.style.width = '100%';
    let i = 0;
    const typing = setInterval(() => {
      if (i < text.length) {
        typewriterText.textContent += text.charAt(i);
        i++;
      } else {
        clearInterval(typing);
      }
    }, 100);
  }, 1000);
}

// Parallax suave no scroll
let ticking = false;
window.addEventListener('scroll', () => {
  if (!ticking) {
    window.requestAnimationFrame(() => {
      const scrolled = window.pageYOffset;
      const parallaxBg = document.querySelector('.particles-bg');
      if (parallaxBg) {
        parallaxBg.style.transform = `translate3d(0, ${scrolled * 0.5}px, 0)`;
      }
      ticking = false;
    });
    ticking = true;
  }
});

// Intersection Observer para animações ao entrar na viewport
const observerOptions = {
  threshold: 0.2,
  rootMargin: '0px 0px -100px 0px'
};

const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.style.opacity = '1';
      entry.target.style.transform = 'translateY(0)';
    }
  });
}, observerOptions);

// Observa todos os cards e elementos animáveis
document.querySelectorAll('.interest-card, .social-card').forEach(el => {
  el.style.opacity = '0';
  el.style.transform = 'translateY(30px)';
  el.style.transition = 'all 0.6s ease';
  observer.observe(el);
});

// Easter Egg: Konami Code
let konamiCode = ['ArrowUp', 'ArrowUp', 'ArrowDown', 'ArrowDown', 'ArrowLeft', 'ArrowRight', 'ArrowLeft', 'ArrowRight', 'b', 'a'];
let konamiIndex = 0;

document.addEventListener('keydown', (e) => {
  if (e.key === konamiCode[konamiIndex]) {
    konamiIndex++;
    if (konamiIndex === konamiCode.length) {
      // Easter Egg ativado!
      document.body.style.animation = 'rainbow 2s linear infinite';
      setTimeout(() => {
        alert('🎉 Easter Egg encontrado! Você é curioso(a) hein! 🚀');
        document.body.style.animation = '';
      }, 100);
      konamiIndex = 0;
    }
  } else {
    konamiIndex = 0;
  }
});

// Animação rainbow para easter egg
const style = document.createElement('style');
style.textContent = `
  @keyframes rainbow {
    0% { filter: hue-rotate(0deg); }
    100% { filter: hue-rotate(360deg); }
  }
`;
document.head.appendChild(style);
</script>
