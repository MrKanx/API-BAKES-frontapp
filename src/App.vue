<script setup lang="ts">
// Mokalu - Awwwards Style Landing Page
</script>

<template>
  <div class="smooth-scroll-wrapper">
    <!-- HERO SECTION -->
    <section class="hero">
      <div class="hero-bg" style="background-image: url('/images/hero.png');"></div>
      <div class="hero-overlay"></div>
      
      <nav class="nav">
        <div class="logo">MOKALÚ.</div>
        <a href="#contacto" class="btn-contact">Hablemos</a>
      </nav>

      <div class="hero-content">
        <div class="reveal-text">
          <h1 class="display-title">TIENDA <br/> DE ARTE</h1>
        </div>
        <p class="hero-subtitle">Materiales premium y piezas personalizadas <br/> para mentes creativas.</p>
      </div>

      <div class="scroll-indicator">
        <div class="mouse"></div>
        <span>Descubre</span>
      </div>
    </section>

    <!-- MARQUEE -->
    <div class="marquee-container">
      <div class="marquee">
        <span>CREATIVIDAD SIN LÍMITES &mdash; ARTE PERSONALIZADO &mdash; MATERIALES PREMIUM &mdash; INSPIRACIÓN DIARIA &mdash; </span>
        <span>CREATIVIDAD SIN LÍMITES &mdash; ARTE PERSONALIZADO &mdash; MATERIALES PREMIUM &mdash; INSPIRACIÓN DIARIA &mdash; </span>
      </div>
    </div>

    <!-- PORTFOLIO / GALLERY -->
    <section class="gallery">
      <div class="gallery-header">
        <h2 class="section-title">NUESTRA <br/> ESENCIA</h2>
        <p class="section-desc">Desde los lienzos más finos hasta zapatillas intervenidas. En Mokalú respiramos arte en cada detalle.</p>
      </div>

      <div class="gallery-grid">
        <div class="gallery-item large">
          <div class="image-wrapper">
            <img src="/images/sneakers.png" alt="Zapatillas Personalizadas" />
            <div class="item-overlay">
              <h3>Arte Único</h3>
              <p>Zapatillas Personalizadas</p>
            </div>
          </div>
        </div>
        <div class="gallery-item">
          <div class="image-wrapper">
            <img src="/images/supplies.png" alt="Materiales de Arte" />
            <div class="item-overlay">
              <h3>Herramientas</h3>
              <p>Papelería Premium</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- FOOTER / LEGAL INFO -->
    <footer id="contacto" class="legal-footer">
      <div class="footer-grid">
        <!-- Branding / Contact -->
        <div class="footer-col brand-col">
          <h2 class="footer-logo">MOKALÚ.</h2>
          <p class="contact-email"><a href="mailto:mokaluventas@gmail.com">mokaluventas@gmail.com</a></p>
          <p class="contact-email"><a href="mailto:lamg5208@gmail.com">lamg5208@gmail.com</a></p>
          <div class="phones">
            <a href="tel:0967472310">0967472310</a> &mdash; 
            <a href="tel:0983849378">0983849378</a>
          </div>
          <p class="copyright">&copy; {{ new Date().getFullYear() }} MOKALU S.A.S. All rights reserved.</p>
        </div>

        <!-- SRI Legal Data -->
        <div class="footer-col legal-data">
          <h4>Información Comercial y Tributaria</h4>
          <div class="data-grid">
            <div class="data-item">
              <span class="label">Razón Social</span>
              <span class="value">MOKALU S.A.S.</span>
            </div>
            <div class="data-item">
              <span class="label">RUC</span>
              <span class="value">0993285811001</span>
            </div>
            <div class="data-item">
              <span class="label">Representante</span>
              <span class="value">Oyola Galarza Monica Alexandra</span>
            </div>
            <div class="data-item">
              <span class="label">Estado / Régimen</span>
              <span class="value">Activo / RIMPE Emprendedor</span>
            </div>
            <div class="data-item">
              <span class="label">Actividades</span>
              <span class="value">Venta al por mayor y menor de artículos de papelería especializada.</span>
            </div>
            <div class="data-item">
              <span class="label">Fechas SRI</span>
              <span class="value">Constitución: 20/10/2020 | Inicio: 23/10/2020</span>
            </div>
            <div class="data-item">
              <span class="label">Verificación SRI</span>
              <span class="value">CATRCR2022002933710</span>
            </div>
          </div>
        </div>

        <!-- Address -->
        <div class="footer-col address-col">
          <h4>Ubicación</h4>
          <p>
            Vía a la Costa Km 12.5,<br>
            C.C. Laguna Plaza, Local 317<br>
            (Primer piso alto junto al ascensor)<br>
            Guayaquil, Guayas, Zona 8<br>
            Ecuador
          </p>
          
          <div class="tax-tags">
            <span class="tax-tag">IVA</span>
            <span class="tax-tag">Renta Sociedades</span>
            <span class="tax-tag">ATS</span>
            <span class="tax-tag">ADI</span>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=Inter:wght@300;400;500&display=swap');

$font-display: 'Syne', sans-serif;
$font-body: 'Inter', sans-serif;
$color-bg: #0a0a0a;
$color-text: #ffffff;
$color-accent: #f2295b;
$color-muted: #888888;

.smooth-scroll-wrapper {
  background-color: $color-bg;
  color: $color-text;
  font-family: $font-body;
  overflow-x: hidden;
  -webkit-font-smoothing: antialiased;
}

/* HERO SECTION */
.hero {
  position: relative;
  height: 100vh;
  width: 100vw;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 2rem 4rem;
  box-sizing: border-box;
  overflow: hidden;

  .hero-bg {
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background-size: cover;
    background-position: center;
    transform: scale(1.05);
    animation: slowZoom 20s infinite alternate linear;
    z-index: 1;
  }

  .hero-overlay {
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: linear-gradient(180deg, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0.8) 100%);
    z-index: 2;
  }

  .nav {
    position: relative;
    z-index: 10;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .logo {
      font-family: $font-display;
      font-weight: 800;
      font-size: 1.5rem;
      letter-spacing: -0.02em;
    }

    .btn-contact {
      border: 1px solid rgba(255,255,255,0.3);
      padding: 0.75rem 1.5rem;
      border-radius: 50px;
      color: $color-text;
      text-decoration: none;
      font-size: 0.9rem;
      transition: all 0.3s ease;
      backdrop-filter: blur(5px);

      &:hover {
        background: $color-text;
        color: $color-bg;
      }
    }
  }

  .hero-content {
    position: relative;
    z-index: 10;
    margin-bottom: 10vh;

    .reveal-text {
      overflow: hidden;
      .display-title {
        font-family: $font-display;
        font-size: clamp(4rem, 12vw, 10rem);
        font-weight: 800;
        line-height: 0.9;
        margin: 0;
        text-transform: uppercase;
        letter-spacing: -0.04em;
        animation: revealUp 1s cubic-bezier(0.77, 0, 0.175, 1) forwards;
      }
    }

    .hero-subtitle {
      margin-top: 2rem;
      font-size: clamp(1rem, 2vw, 1.5rem);
      font-weight: 300;
      opacity: 0;
      animation: fadeIn 1s ease 1s forwards;
    }
  }

  .scroll-indicator {
    position: absolute;
    bottom: 2rem;
    left: 50%;
    transform: translateX(-50%);
    z-index: 10;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    opacity: 0.7;

    .mouse {
      width: 20px;
      height: 30px;
      border: 1px solid white;
      border-radius: 10px;
      position: relative;

      &::after {
        content: '';
        position: absolute;
        top: 5px;
        left: 50%;
        transform: translateX(-50%);
        width: 2px;
        height: 5px;
        background: white;
        border-radius: 2px;
        animation: scrollWheel 2s infinite ease-in-out;
      }
    }
  }
}

/* MARQUEE */
.marquee-container {
  padding: 4rem 0;
  background: $color-accent;
  color: $color-bg;
  overflow: hidden;
  white-space: nowrap;

  .marquee {
    display: inline-block;
    animation: marqueeMove 20s linear infinite;
    
    span {
      font-family: $font-display;
      font-weight: 800;
      font-size: 3rem;
      padding-right: 1rem;
    }
  }
}

/* GALLERY */
.gallery {
  padding: 10vw 4rem;

  .gallery-header {
    margin-bottom: 5rem;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    gap: 2rem;
    flex-wrap: wrap;

    .section-title {
      font-family: $font-display;
      font-size: clamp(3rem, 8vw, 6rem);
      line-height: 0.9;
      margin: 0;
    }

    .section-desc {
      max-width: 400px;
      font-size: 1.1rem;
      color: $color-muted;
      line-height: 1.6;
    }
  }

  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    gap: 2rem;

    .gallery-item {
      position: relative;
      overflow: hidden;
      border-radius: 8px;
      cursor: pointer;

      &.large {
        grid-column: span 7;
      }
      &:not(.large) {
        grid-column: span 5;
        margin-top: 10vw;
      }

      .image-wrapper {
        width: 100%;
        height: 100%;
        position: relative;

        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          transition: transform 0.7s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }

        .item-overlay {
          position: absolute;
          inset: 0;
          background: rgba(0,0,0,0.4);
          display: flex;
          flex-direction: column;
          justify-content: flex-end;
          padding: 2rem;
          opacity: 0;
          transition: opacity 0.4s ease;

          h3 {
            font-family: $font-display;
            font-size: 2rem;
            margin: 0 0 0.5rem;
          }
          p {
            margin: 0;
            font-size: 1rem;
            color: #ddd;
          }
        }
      }

      &:hover {
        .image-wrapper img {
          transform: scale(1.05);
        }
        .item-overlay {
          opacity: 1;
        }
      }
    }
  }
}

/* FOOTER */
.legal-footer {
  background: #050505;
  padding: 6rem 4rem 2rem;
  border-top: 1px solid rgba(255,255,255,0.1);

  .footer-grid {
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    gap: 4rem;

    .footer-col {
      h4 {
        font-family: $font-display;
        font-size: 1.2rem;
        margin-bottom: 1.5rem;
        color: #fff;
        font-weight: 700;
      }
      p {
        color: $color-muted;
        font-size: 0.85rem;
        line-height: 1.6;
        margin-bottom: 0.5rem;
      }
      a {
        color: $color-muted;
        text-decoration: none;
        transition: color 0.3s;
        &:hover { color: $color-text; }
      }
    }

    .brand-col {
      .footer-logo {
        font-family: $font-display;
        font-size: 2rem;
        margin: 0 0 1rem;
      }
      .phones {
        font-size: 0.85rem;
        color: $color-muted;
        margin-bottom: 2rem;
      }
      .copyright {
        margin-top: 3rem;
        font-size: 0.75rem;
        opacity: 0.5;
      }
    }

    .legal-data {
      .data-grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 1.5rem 2rem;
        
        .data-item {
          display: flex;
          flex-direction: column;
          gap: 0.2rem;

          .label {
            font-size: 0.7rem;
            text-transform: uppercase;
            letter-spacing: 0.05em;
            color: #555;
          }
          .value {
            font-size: 0.85rem;
            color: #ccc;
          }
        }
      }
    }

    .address-col {
      .tax-tags {
        margin-top: 2rem;
        display: flex;
        flex-wrap: wrap;
        gap: 0.5rem;

        .tax-tag {
          font-size: 0.65rem;
          padding: 0.2rem 0.5rem;
          border: 1px solid #333;
          border-radius: 4px;
          color: #aaa;
        }
      }
    }
  }
}

/* ANIMATIONS */
@keyframes slowZoom {
  0% { transform: scale(1) translate(0, 0); }
  100% { transform: scale(1.1) translate(-2%, 2%); }
}
@keyframes revealUp {
  0% { transform: translateY(100%); opacity: 0; }
  100% { transform: translateY(0); opacity: 1; }
}
@keyframes fadeIn {
  to { opacity: 1; }
}
@keyframes scrollWheel {
  0% { transform: translate(-50%, 0); opacity: 1; }
  100% { transform: translate(-50%, 15px); opacity: 0; }
}
@keyframes marqueeMove {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}

/* RESPONSIVE */
@media (max-width: 1024px) {
  .hero { padding: 2rem; }
  .gallery { padding: 5vw 2rem; }
  .legal-footer .footer-grid {
    grid-template-columns: 1fr;
    gap: 3rem;
  }
  .gallery .gallery-grid {
    .gallery-item {
      &.large, &:not(.large) {
        grid-column: span 12;
        margin-top: 0;
      }
    }
  }
}
@media (max-width: 768px) {
  .legal-footer .legal-data .data-grid {
    grid-template-columns: 1fr;
  }
}
</style>
