---
title: "Minhas Habilidades"
permalink: /habilidades/
layout: single
---

<style>
/* ==================== FUNDO AZUL PARA INITIAL-CONTENT ==================== */
.initial-content {
  background: linear-gradient(145deg, rgba(20, 40, 80, 0.8), rgba(10, 20, 40, 0.9));
}

/* ==================== FUNDO NEON ANIMADO PARA HABILIDADES ==================== */
body.page--habilidades {
  background: #142850;
  overflow-x: hidden;
}

/* Camada neon animada nos blocos */
.notice--info,
.notice--success,
.notice--warning {
  background: linear-gradient(145deg, rgba(20, 40, 80, 0.8), rgba(10, 20, 40, 0.9));
  border-radius: 15px;
  padding: 30px 25px;
  margin-bottom: 25px;
  position: relative;
  overflow: hidden;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.5);
  transition: all 0.4s ease;
}

.notice--info::before,
.notice--success::before,
.notice--warning::before,
.initial-content::before {
  content: "";
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: linear-gradient(135deg, #4da6ff, #00ccff, #4da6ff, #00ccff);
  opacity: 0.2;
  transform: rotate(45deg);
  filter: blur(40px);
  animation: neonGlow 6s linear infinite;
  pointer-events: none;
  z-index: 0;
  border-radius: 20px;
}

/* Hover nos blocos */
.notice--info:hover,
.notice--success:hover,
.notice--warning:hover,
.initial-content:hover {
  box-shadow: 0 15px 50px rgba(77, 166, 255, 0.5);
  transform: translateY(-5px) scale(1.02);
}

/* ==================== TÍTULOS EM NEON ==================== */
.page__title,
h2, h3 {
  text-align: center;
  font-size: 48px;
  font-weight: 700;
  background: linear-gradient(90deg, #4da6ff, #00ccff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  color: #ffffff;
  text-shadow: 2px 2px 10px rgba(77, 166, 255, 0.5);
  margin-bottom: 30px;
}

/* Títulos dentro dos blocos */
.notice--info h4,
.notice--success h4,
.notice--warning h4 {
  position: relative;
  z-index: 1;
  color: #4da6ff;
  text-shadow:
    0 0 5px #4da6ff,
    0 0 10px #00ccff,
    0 0 20px #00ccff,
    0 0 40px #0088cc;
  margin-bottom: 10px;
}

/* ==================== ITENS DE LISTA COM BOLINHA NEON ==================== */
/* Apenas nas listas dentro de notice */
.notice--info li,
.notice--success li,
.notice--warning li {
  position: relative;
  z-index: 1;
  color: #cccccc;
  padding-left: 20px;
  margin-bottom: 8px;
}

.notice--info li::before,
.notice--success li::before,
.notice--warning li::before {
  content: "•";
  position: absolute;
  left: 0;
  color: #4da6ff;
  font-weight: bold;
  text-shadow:
    0 0 3px #4da6ff,
    0 0 6px #00ccff,
    0 0 10px #00ccff;
}

/* ==================== ANIMAÇÃO NEON ==================== */
@keyframes neonGlow {
  0%, 100% {
    transform: rotate(0deg) translate(-50%, -50%);
  }
  50% {
    transform: rotate(45deg) translate(-50%, -50%);
  }
}

/* ==================== RESPONSIVO ==================== */
@media (max-width: 768px) {
  .initial-content,
  .notice--info,
  .notice--success,
  .notice--warning {
    padding: 20px 15px;
  }

  .page__title,
  h2, h3 {
    font-size: 36px;
  }

  .notice--info h4,
  .notice--success h4,
  .notice--warning h4 {
    font-size: 20px;
  }
}
</style>







## 💻 Principais Habilidades

<div class="notice--info">
  <h4>Infraestrutura & Redes</h4>
  <ul>
    <li>Configuração de switches, routers e firewalls</li>
    <li>Mikrotik, TP-Link</li>
    <li>Protocolos: TCP/IP, VLANs, OSPF, BGP</li>
    <li>Segurança de rede e VPN</li>
  </ul>
</div>

<div class="notice--success">
  <h4>Sistemas & Virtualização</h4>
  <ul>
    <li>Linux (Slackware, Ubuntu, CentOS)</li>
    <li>Windows Server (2016/2019/2022)</li>
    <li>VMware vSphere & Hyper-V</li>
  </ul>
</div>

<div class="notice--warning">
  <h4>Automação & Scripting</h4>
  <ul>
    <li>PowerShell para automação Windows</li>
    <li>Bash scripting para Linux</li>
    <li>Python para automação de tarefas</li>
  </ul>
</div>
