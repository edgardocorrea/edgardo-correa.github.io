<style>
/* ============================================================
   FUNDO GERAL DA PÁGINA (com movimento neon leve)
   ============================================================ */
body.page--certificacoes {
  background: #142850 !important;
  overflow-x: hidden;
}

.initial-content {
  position: relative;
  background: linear-gradient(145deg, rgba(20,40,80,0.8), rgba(10,20,40,0.9));
  padding: 30px 25px;
  border-radius: 15px;
  box-shadow: 0 8px 25px rgba(0,0,0,0.6);
  overflow: hidden;
}

/* Movimento neon no fundo */
.initial-content::before {
  content: "";
  position: absolute;
  top: -40%;
  left: -40%;
  width: 180%;
  height: 180%;
  background: linear-gradient(135deg, #4da6ff, #00ccff, #4da6ff);
  filter: blur(60px);
  opacity: 0.18;
  animation: neonMove 10s linear infinite;
  z-index: 0;
}
@keyframes neonMove {
  0% { transform: rotate(0deg) translate(0,0); }
  50% { transform: rotate(45deg) translate(80px, 80px); }
  100% { transform: rotate(0deg) translate(0,0); }
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
  text-shadow: 2px 2px 12px rgba(77, 166, 255, 0.7);
  margin-bottom: 25px;
}

/* ============================================================
   CARDS DE CERTIFICADO (com neon e movimento)
   ============================================================ */
.cert-card {
  background: linear-gradient(145deg, rgba(20,40,80,0.85), rgba(10,20,40,0.95));
  border-radius: 15px;
  padding: 25px;
  margin-bottom: 25px;
  position: relative;
  overflow: hidden;
  transition: 0.4s ease;
  box-shadow: 0 6px 20px rgba(0,0,0,0.5);
}

/* Camada neon animada */
.cert-card::before {
  content: "";
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: linear-gradient(135deg, #4da6ff, #00ccff, #4da6ff, #00ccff);
  filter: blur(50px);
  opacity: 0.2;
  animation: neonCardMove 8s linear infinite;
  z-index: 0;
}
@keyframes neonCardMove {
  0% { transform: rotate(0deg) translate(-50%, -50%); }
  50% { transform: rotate(45deg) translate(-30%, -30%); }
  100% { transform: rotate(0deg) translate(-50%, -50%); }
}

/* Hover neon */
.cert-card:hover {
  transform: translateY(-6px) scale(1.02);
  box-shadow: 0 15px 55px rgba(77, 166, 255, 0.7);
}

/* ============================================================
   TÍTULOS EM NEON (Categorias e nomes dos certificados)
   ============================================================ */
.cert-section-title,
.cert-title,
h2, h3, h4 {
  position: relative;
  z-index: 2;
  color: #ffffff !important;
  font-weight: 700;
  text-shadow:
    0 0 8px #4da6ff,
    0 0 16px #00ccff,
    0 0 32px #4da6ff;
}

/* ============================================================
   TEXTOS DENTRO DOS CARDS
   ============================================================ */
.cert-description,
.cert-provider,
.cert-card p {
  position: relative;
  z-index: 2;
  color: #cccccc;
}

/* ============================================================
   LISTAS (somente dentro dos cards)
   ============================================================ */
.cert-card ul li {
  position: relative;
  z-index: 2;
  color: #e0e0e0;
  padding-left: 15px;
  margin-bottom: 6px;
}

.cert-card ul li::before {
  content: "•";
  position: absolute;
  left: 0;
  font-size: 18px;
  color: #4da6ff;
  text-shadow: 
    0 0 5px #4da6ff,
    0 0 12px #00ccff;
}

/* ============================================================
   RESPONSIVO
   ============================================================ */
@media (max-width: 768px) {
  .page__title {
    font-size: 36px !important;
  }
  .cert-card {
    padding: 20px;
  }
}
</style>
