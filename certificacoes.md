---
title: "Certificações e Badges"
permalink: /certificacoes/
layout: single
---

<style>
/* ==================== FUNDO NORMAL PARA A PÁGINA ================================= */
body.page--certificacoes,
body.page--certificacoes main.grid__item {
  background: #142850;  /* azul escuro padrão */
  color: #cccccc;
}

/* ==================== BADGE DE CERTIFICADO – ESTILO DE CARD NEON ===================== */
/* Supondo que os certificados usam a classe `.cert-card` */
.cert-card {
  background: linear-gradient(145deg, rgba(20,40,80,0.8), rgba(10,20,40,0.9));
  border-radius: 15px;
  padding: 30px;
  margin: 20px 0;
  position: relative;
  overflow: hidden;
  box-shadow: 0 8px 30px rgba(0,0,0,0.5);
  transition: all 0.4s ease;
}

/* Camada de brilho/neon nos cartões */
.cert-card::before {
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

/* Hover para destacar */
.cert-card:hover {
  box-shadow: 0 15px 50px rgba(77,166,255,0.5);
  transform: translateY(-5px) scale(1.02);
}

/* ==================== TÍTULO DA PÁGINA EM NEON ======================================= */
.page__title {
  text-align: center;
  font-size: 48px !important;
  background: linear-gradient(90deg, #4da6ff, #00ccff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  color: #ffffff;
  text-shadow: 2px 2px 10px rgba(77,166,255,0.5);
  margin-bottom: 20px;
}

/* ==================== ITENS DENTRO DO CARD =========================================== */
/* Suponha que dentro do badge tenha `.cert-title`, `.cert-description` */
.cert-title {
  position: relative;
  z-index: 1;
  color: #ffffff;
  font-size: 24px;
  margin-bottom: 10px;
}

.cert-description {
  position: relative;
  z-index: 1;
  color: #cccccc;
  font-size: 16px;
  line-height: 1.6;
}

/* ==================== ANIMAÇÃO NEON ================================================== */
@keyframes neonGlow {
  0%, 100% { transform: rotate(0deg) translate(-50%, -50%); }
  50% { transform: rotate(45deg) translate(-50%, -50%); }
}

/* ==================== RESPONSIVO ==================================================== */
@media (max-width: 768px) {
  .cert-card {
    padding: 25px;
  }
  .page__title {
    font-size: 36px !important;
  }
  .cert-title {
    font-size: 20px;
  }
}
</style>


Nesta página, apresento as minhas certificações profissionais, que validam as minhas competências em diversas áreas da tecnologia. Para mais detalhes ou para verificar a autenticidade, visite meu perfil completo no [Credly](https://www.credly.com/users/edgardo.correa).

---

## Redes

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="232a032a-8675-4fbd-9752-b74219f08ad8" data-share-badge-host="https://www.credly.com"></div>

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="5c6077c7-6f57-4196-b648-e7d3b5b82624" data-share-badge-host="https://www.credly.com"></div>

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="e0ee1601-18f3-41d2-97f3-67a836bfe4c9" data-share-badge-host="https://www.credly.com"></div>

---

## Segurança da Informação

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="d44d5772-1fee-4491-9326-ab1aa4a908ca" data-share-badge-host="https://www.credly.com"></div>

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="02abd07a-71a8-4024-8316-0dd40691fa74" data-share-badge-host="https://www.credly.com"></div>

---

## Inteligência Artificial e Metodologias Ágeis

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="aa5e1665-af74-4d59-9567-409b890991f4" data-share-badge-host="https://www.credly.com"></div>

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="bdb8bcd3-8357-4d2e-8894-f1fe4e36e079" data-share-badge-host="https://www.credly.com"></div>

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="24f3cc92-a5fb-469b-820d-d2d85b4d487c" data-share-badge-host="https://www.credly.com"></div>

<!-- Script do Credly para renderizar todos os badges acima. Apenas um é necessário por página. -->
<script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>
