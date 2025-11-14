---
title: "Certificações e Badges"
permalink: /certificacoes/
layout: single
---

<style>
/* ============================================================
   FUNDO COMPLETO DA PÁGINA COM MOVIMENTO
============================================================ */
body.page--certificacoes {
  background: #142850 !important;
  overflow-x: hidden;
  position: relative;
}

body.page--certificacoes::before {
  content: "";
  position: fixed;
  top: -30%;
  left: -30%;
  width: 160%;
  height: 160%;
  background: linear-gradient(135deg, #4da6ff, #00ccff, #4da6ff);
  filter: blur(120px);
  opacity: 0.15;
  animation: bgMove 16s linear infinite;
  z-index: 0;
}

@keyframes bgMove {
  0% { transform: rotate(0deg) translate(0,0); }
  50% { transform: rotate(35deg) translate(150px, 150px); }
  100% { transform: rotate(0deg) translate(0,0); }
}

/* ============================================================
   CONTEÚDO PRINCIPAL
============================================================ */
.initial-content {
  position: relative;
  background: rgba(10,20,40,0.85);
  padding: 30px 25px;
  border-radius: 20px;
  backdrop-filter: blur(3px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.6);
  z-index: 2;
  overflow: hidden;
}

/* Texto "Nesta página..." */
.initial-content p,
.initial-content strong,
.initial-content a {
  color: #ffffff !important;
  text-shadow: none !important;
}

/* ============================================================
   TÍTULO PRINCIPAL EM NEON
============================================================ */
.page__title {
  text-align: center;
  font-size: 48px !important;
  background: linear-gradient(90deg, #4da6ff, #00ccff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  text-shadow: 0 0 12px rgba(77,166,255,0.7);
  margin-bottom: 25px;
}

/* ============================================================
   TÍTULOS DAS SEÇÕES (Redes / Segurança / IA)
   → brancos, sem neon
============================================================ */
.initial-content h2,
.initial-content h3 {
  color: #ffffff !important;
  text-shadow: none !important;
  font-weight: 700;
  margin-top: 35px;
  margin-bottom: 12px;
  position: relative;
  z-index: 3;
}

/* ============================================================
   BADGES DO CREDLY — ENVOLTÓRIO NEON
============================================================ */
.credly-badge-wrapper {
  display: inline-block;
  padding: 10px;
  border-radius: 16px;
  background: rgba(20,40,80,0.85);
  margin: 12px;
  position: relative;
  box-shadow:
    0 0 8px #4da6ff66,
    0 0 16px #00ccff44;
  transition: 0.3s ease-in-out;
}

.credly-badge-wrapper:hover {
  transform: scale(1.06);
  box-shadow:
    0 0 14px #4da6ffcc,
    0 0 28px #00ccff99;
}

.credly-badge-wrapper iframe {
  border-radius: 12px !important;
  border: 2px solid #4da6ff !important;
}

/* ============================================================
   RESPONSIVO
============================================================ */
@media (max-width: 768px) {
  .page__title { font-size: 36px !important; }
}
</style>


Nesta página, apresento as minhas certificações profissionais, que validam as minhas competências em diversas áreas da tecnologia.  
Para consultar todas as certificações diretamente, acesse meu perfil no  
**[Credly](https://www.credly.com/users/edgardo.correa)**.

---

## Redes

<div class="credly-badge-wrapper">
  <div data-iframe-width="150" data-iframe-height="270"
    data-share-badge-id="232a032a-8675-4fbd-9752-b74219f08ad8"
    data-share-badge-host="https://www.credly.com"></div>
</div>

<div class="credly-badge-wrapper">
  <div data-iframe-width="150" data-iframe-height="270"
    data-share-badge-id="5c6077c7-6f57-4196-b648-e7d3b5b82624"
    data-share-badge-host="https://www.credly.com"></div>
</div>

<div class="credly-badge-wrapper">
  <div data-iframe-width="150" data-iframe-height="270"
    data-share-badge-id="e0ee1601-18f3-41d2-97f3-67a836bfe4c9"
    data-share-badge-host="https://www.credly.com"></div>
</div>

---

## Segurança da Informação

<div class="credly-badge-wrapper">
  <div data-iframe-width="150" data-iframe-height="270"
    data-share-badge-id="d44d5772-1fee-4491-9326-ab1aa4a908ca"
    data-share-badge-host="https://www.credly.com"></div>
</div>

<div class="credly-badge-wrapper">
  <div data-iframe-width="150" data-iframe-height="270"
    data-share-badge-id="02abd07a-71a8-4024-8316-0dd40691fa74"
    data-share-badge-host="https://www.credly.com"></div>
</div>

---

## Inteligência Artificial e Metodologias Ágeis

<div class="credly-badge-wrapper">
  <div data-iframe-width="150" data-iframe-height="270"
    data-share-badge-id="aa5e1665-af74-4d59-9567-409b890991f4"
    data-share-badge-host="https://www.credly.com"></div>
</div>

<div class="credly-badge-wrapper">
  <div data-iframe-width="150" data-iframe-height="270"
    data-share-badge-id="bdb8bcd3-8357-4d2e-8894-f1fe4e36e079"
    data-share-badge-host="https://www.credly.com"></div>
</div>

<div class="credly-badge-wrapper">
  <div data-iframe-width="150" data-iframe-height="270"
    data-share-badge-id="24f3cc92-a5fb-469b-820d-d2d85b4d487c"
    data-share-badge-host="https://www.credly.com"></div>
</div>

<!-- Script do Credly -->
<script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>
