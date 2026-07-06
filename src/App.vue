<script setup lang="ts">
// Ohayo Ecuador - Landing Page
</script>

<template>
  <div class="smooth-scroll-wrapper">
    <!-- HERO SECTION -->
    <section class="hero">
      <div class="hero-bg" style="background-image: url('/images/ohayo_hero_bg.png');"></div>
      <div class="hero-overlay"></div>
      
      <nav class="nav">
        <div class="logo">OHAYO ECUADOR</div>
        <a href="#contacto" class="btn-contact">Contacto</a>
      </nav>

      <div class="hero-content">
        <div class="reveal-text">
          <h1 class="display-title">OHAYO <br/> ECUADOR</h1>
        </div>
        <p class="hero-subtitle">Tu portal premium a la cultura otaku y geek en Ecuador. <br/> Figuras originales, literatura manga, katanas coleccionables y accesorios con envíos nacionales.</p>
      </div>

      <div class="scroll-indicator">
        <div class="mouse"></div>
        <span>Desliza para ver</span>
      </div>
    </section>

    <!-- MARQUEE -->
    <div class="marquee-container">
      <div class="marquee">
        <span>FIGURAS DE COLECCIÓN &mdash; LITERATURA MANGA &mdash; NOVELAS LIGERAS &mdash; KATANAS PERSONALIZADAS &mdash; DAKIMAKURAS &mdash; ACCESORIOS GEEK &mdash; ENVÍOS A NIVEL NACIONAL &mdash; </span>
        <span>FIGURAS DE COLECCIÓN &mdash; LITERATURA MANGA &mdash; NOVELAS LIGERAS &mdash; KATANAS PERSONALIZADAS &mdash; DAKIMAKURAS &mdash; ACCESORIOS GEEK &mdash; ENVÍOS A NIVEL NACIONAL &mdash; </span>
      </div>
    </div>

    <!-- PORTFOLIO / GALLERY (CATEGORIES) -->
    <section class="gallery">
      <div class="gallery-header">
        <h2 class="section-title">NUESTRA <br/> PROPUESTA</h2>
        <p class="section-desc">Nos especializamos en la importación y comercialización de productos exclusivos de anime, manga y videojuegos, combinando canales físicos y en línea.</p>
      </div>

      <div class="gallery-grid">
        <div class="gallery-item large">
          <div class="image-wrapper">
            <img src="/images/anime_figures.png" alt="Figuras de Colección" />
            <div class="item-overlay">
              <h3>Figuras de Colección</h3>
              <p>Estatuas a escala y figuras de acción originales de tus series favoritas.</p>
            </div>
          </div>
        </div>
        <div class="gallery-item">
          <div class="image-wrapper">
            <img src="/images/manga_novels.png" alt="Literatura Anime" />
            <div class="item-overlay">
              <h3>Literatura Anime</h3>
              <p>Venta de tomos de manga y novelas ligeras en español e inglés.</p>
            </div>
          </div>
        </div>
        <div class="gallery-item wide">
          <div class="image-wrapper">
            <img src="/images/geek_accessories.png" alt="Accesorios Variados" />
            <div class="item-overlay">
              <h3>Accesorios Variados</h3>
              <p>Cojines Dakimakura, artículos de consolas de videojuegos y mercancía temática general.</p>
            </div>
          </div>
        </div>
        <div class="gallery-item" style="grid-column: span 12; margin-top: 4rem; aspect-ratio: 21 / 9;">
          <div class="image-wrapper">
            <img src="/images/katana_replicas.png" alt="Réplicas Coleccionables" />
            <div class="item-overlay">
              <h3>Réplicas Coleccionables</h3>
              <p>Katanas personalizadas inspiradas en personajes icónicos.</p>
            </div>
          </div>
        </div>
      </div>
    </section>



    <!-- FOOTER -->
    <footer id="contacto" class="legal-footer">
      <div class="footer-grid">
        <!-- Branding / Contact -->
        <div class="footer-col brand-col">
          <h2 class="footer-logo">OHAYO ECUADOR</h2>
          <p class="contact-email"><a href="mailto:brandoncoellomoreira@gmail.com">brandoncoellomoreira@gmail.com</a></p>
          <div class="phones">
            <a href="tel:0995076954">0995076954</a>
          </div>
          <p class="copyright">&copy; 2026 BRANDON SANTIAGO COELLO MOREIRA. Todos los derechos reservados.</p>
        </div>

        <!-- Verification Summary Quick -->
        <div class="footer-col legal-data">
          <h4>Resumen de Negocio</h4>
          <div class="data-grid">
            <div class="data-item">
              <span class="label">Propietario</span>
              <span class="value">BRANDON SANTIAGO COELLO MOREIRA</span>
            </div>
            <div class="data-item">
              <span class="label">RUC</span>
              <span class="value">0952265528001</span>
            </div>
            <div class="data-item">
              <span class="label">Régimen</span>
              <span class="value">RIMPE - Negocio Popular</span>
            </div>
            <div class="data-item">
              <span class="label">Obligado Contabilidad</span>
              <span class="value">NO</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Actividad SRI Principal</span>
              <span class="value">Venta al por mayor de otros productos diversos para el consumidor</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Código Certificado RUC</span>
              <span class="value">RCR1781740466673260 (Emisión 17/Jun/2026)</span>
            </div>
          </div>
        </div>

        <!-- Address / Location -->
        <div class="footer-col address-col">
          <h4>Domicilio y Tienda</h4>
          <p>
            Provincia: Guayas<br>
            Cantón: Guayaquil<br>
            Parroquia: Tarqui<br>
            Barrio Garzota 2, Calle Washington Delgado C.,<br>
            Villa 8, Intersección 14 Pasaje 3 NE.<br>
            <strong>Referencia:</strong> A una cuadra del gimnasio Vikingos.
          </p>
          <div class="tax-badges">
            <span class="badge">RUC Activo</span>
            <span class="badge">RIMPE</span>
            <span class="badge">E-Commerce & Físico</span>
          </div>
        </div>
      </div>

      <div class="footer-bottom">
        <p class="developer-credit">
          Hecho por <a href="https://github.com/MrKanx" target="_blank" rel="noopener noreferrer">Kankox</a>
        </p>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=Inter:wght@300;400;500;700&display=swap');

$font-display: 'Syne', sans-serif;
$font-body: 'Inter', sans-serif;
$color-bg: #06050b; // Deep night violet
$color-card: #110d1e; // Purple night card
$color-text: #f3effa; // Warm off-white
$color-accent: #ff2a5f; // Neon pink/magenta
$color-secondary: #00e5ff; // Neon cyan
$color-muted: #9f95b5; // Muted lavender

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
    background: linear-gradient(180deg, rgba($color-bg, 0.3) 0%, rgba($color-bg, 0.9) 100%);
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
      background: linear-gradient(90deg, $color-accent, $color-secondary);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .btn-contact {
      border: 1px solid rgba(255,255,255,0.15);
      padding: 0.75rem 1.5rem;
      border-radius: 50px;
      color: $color-text;
      text-decoration: none;
      font-size: 0.9rem;
      transition: all 0.3s ease;
      backdrop-filter: blur(5px);

      &:hover {
        background: $color-accent;
        color: #fff;
        border-color: $color-accent;
        box-shadow: 0 0 15px rgba($color-accent, 0.4);
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
        font-size: clamp(3.5rem, 11vw, 9rem);
        font-weight: 800;
        line-height: 0.9;
        margin: 0;
        text-transform: uppercase;
        letter-spacing: -0.04em;
        animation: revealUp 1s cubic-bezier(0.77, 0, 0.175, 1) forwards;
        background: linear-gradient(135deg, #fff 30%, $color-muted);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }
    }

    .hero-subtitle {
      margin-top: 2rem;
      font-size: clamp(1rem, 2vw, 1.35rem);
      font-weight: 300;
      opacity: 0;
      animation: fadeIn 1s ease 1s forwards;
      color: #dfd7ee;
      line-height: 1.6;
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
  padding: 3rem 0;
  background: #0d091a;
  border-top: 1px solid rgba($color-secondary, 0.15);
  border-bottom: 1px solid rgba($color-secondary, 0.15);
  color: #fff;
  overflow: hidden;
  white-space: nowrap;
  box-shadow: 0 0 20px rgba($color-secondary, 0.03);

  .marquee {
    display: inline-block;
    animation: marqueeMove 25s linear infinite;
    
    span {
      font-family: $font-display;
      font-weight: 800;
      font-size: 2.2rem;
      padding-right: 2rem;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      background: linear-gradient(90deg, $color-accent, $color-secondary);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
  }
}

/* GALLERY (CATEGORIES) */
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
      border-radius: 12px;
      cursor: pointer;
      aspect-ratio: 4 / 3;
      border: 1px solid rgba(255, 255, 255, 0.05);

      &.large {
        grid-column: span 7;
        aspect-ratio: 16 / 10;
      }
      &.wide {
        grid-column: span 12;
        aspect-ratio: 21 / 9;
        margin-top: 4rem;
      }
      &:not(.large):not(.wide) {
        grid-column: span 5;
        margin-top: 10vw;
        aspect-ratio: 4 / 5;
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
          background: linear-gradient(to top, rgba($color-bg, 0.9) 10%, rgba(0,0,0,0.2) 100%);
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
            color: #fff;
          }
          p {
            margin: 0;
            font-size: 1rem;
            color: #ccc;
            line-height: 1.4;
          }
        }
      }

      &:hover {
        border-color: rgba($color-secondary, 0.3);
        box-shadow: 0 10px 30px rgba(0,0,0,0.5);

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
  background: darken($color-bg, 3%);
  padding: 6rem 4rem 2rem;
  border-top: 1px solid rgba(255,255,255,0.05);

  .footer-grid {
    display: grid;
    grid-template-columns: 1.2fr 1.8fr 1.2fr;
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
        background: linear-gradient(90deg, $color-accent, $color-secondary);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }
      .phones {
        font-size: 0.85rem;
        color: $color-muted;
        margin-bottom: 2rem;
        
        a {
          color: $color-secondary;
          font-weight: 700;
        }
      }
      .copyright {
        margin-top: 3rem;
        font-size: 0.75rem;
        opacity: 0.5;
      }
    }

    .address-col {
      .tax-badges {
        display: flex;
        gap: 0.5rem;
        margin-top: 1.5rem;
        flex-wrap: wrap;

        .badge {
          font-size: 0.7rem;
          padding: 0.25rem 0.5rem;
          border: 1px solid rgba(255, 255, 255, 0.15);
          border-radius: 4px;
          color: $color-muted;
          text-transform: uppercase;
          letter-spacing: 0.05em;
          transition: all 0.3s ease;
          cursor: default;

          &:hover {
            border-color: $color-secondary;
            color: #fff;
            background: rgba($color-secondary, 0.05);
          }
        }
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

          &.span-2 {
            grid-column: span 2;
          }

          .label {
            font-size: 0.7rem;
            text-transform: uppercase;
            letter-spacing: 0.05em;
            color: $color-muted;
          }
          .value {
            font-size: 0.85rem;
            color: #ddd;
          }
        }
      }
    }
  }

  .footer-bottom {
    margin-top: 3rem;
    padding-top: 1.5rem;
    border-top: 1px solid rgba(255, 255, 255, 0.05);
    text-align: center;

    .developer-credit {
      font-size: 0.8rem;
      color: #555;
      letter-spacing: 0.05em;

      a {
        color: #777;
        text-decoration: underline;
        text-underline-offset: 3px;
        transition: color 0.3s ease;

        &:hover {
          color: #ccc;
        }
      }
    }
  }
}

/* ANIMATIONS */
@keyframes slowZoom {
  0% { transform: scale(1) translate(0, 0); }
  100% { transform: scale(1.1) translate(-1%, 1%); }
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
      &.large, &.wide, &:not(.large):not(.wide) {
        grid-column: span 12;
        margin-top: 0;
        aspect-ratio: 16 / 10;
      }
    }
  }
}


</style>
