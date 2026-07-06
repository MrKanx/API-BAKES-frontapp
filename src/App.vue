<script setup lang="ts">
// One Love Coffee Shop - Awwwards Style Landing Page
</script>

<template>
  <div class="smooth-scroll-wrapper">
    <!-- HERO SECTION -->
    <section class="hero">
      <div class="hero-bg" style="background-image: url('/images/onelove_hero_bg.png');"></div>
      <div class="hero-overlay"></div>
      
      <nav class="nav">
        <div class="logo">ONE LOVE COFFEE SHOP</div>
        <a href="#contacto" class="btn-contact">Visítanos</a>
      </nav>

      <div class="hero-content">
        <div class="reveal-text">
          <h1 class="display-title">ONE LOVE <br/> COFFEE SHOP</h1>
        </div>
        <p class="hero-subtitle">Café orgánico de especialidad, gastronomía variada <br/> y buena vibra frente al río en Puerto Santa Ana, Guayaquil.</p>
      </div>

      <div class="scroll-indicator">
        <div class="mouse"></div>
        <span>Descubre más</span>
      </div>
    </section>

    <!-- MARQUEE -->
    <div class="marquee-container">
      <div class="marquee">
        <span>CAFÉ DE ESPECIALIDAD &mdash; BUENA VIBRA &mdash; FILOSOFÍA BOB MARLEY &mdash; OSOS DE PELUCHE GIGANTES &mdash; PUERTO SANTA ANA &mdash; </span>
        <span>CAFÉ DE ESPECIALIDAD &mdash; BUENA VIBRA &mdash; FILOSOFÍA BOB MARLEY &mdash; OSOS DE PELUCHE GIGANTES &mdash; PUERTO SANTA ANA &mdash; </span>
      </div>
    </div>

    <!-- PORTFOLIO / GALLERY -->
    <section class="gallery">
      <div class="gallery-header">
        <h2 class="section-title">NUESTRA <br/> PROPUESTA</h2>
        <p class="section-desc">Un espacio diseñado para relajarse sin prisa. Combinamos café premium 100% arábigo, repostería artesanal y la mejor energía inspirada en Bob Marley.</p>
      </div>

      <div class="gallery-grid">
        <div class="gallery-item large">
          <div class="image-wrapper">
            <img src="/images/specialty_coffee.png" alt="Café de Especialidad" />
            <div class="item-overlay">
              <h3>Café de Especialidad</h3>
              <p>Granos 100% arábigos y orgánicos</p>
            </div>
          </div>
        </div>
        <div class="gallery-item">
          <div class="image-wrapper">
            <img src="/images/gastronomy.png" alt="Gastronomía Variada" />
            <div class="item-overlay">
              <h3>Gastronomía Variada</h3>
              <p>Brunch, postres artesanales y toques locales</p>
            </div>
          </div>
        </div>
        <div class="gallery-item wide">
          <div class="image-wrapper">
            <img src="/images/cozy_atmosphere.png" alt="Ambiente Acogedor" />
            <div class="item-overlay">
              <h3>Ambiente & Estética Acogedora</h3>
              <p>Relájate junto al río en Puerto Santa Ana con la compañía de nuestros osos gigantes</p>
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
          <h2 class="footer-logo">ONE LOVE COFFEE SHOP</h2>
          <p class="contact-email"><a href="mailto:carloslopezpatino@gmail.com">carloslopezpatino@gmail.com</a></p>
          <div class="phones">
            <a href="tel:042852338">042852338</a>
          </div>
          <p class="copyright">&copy; 2026 CARLOS ALFREDO LOPEZ PATIÑO. Todos los derechos reservados.</p>
        </div>

        <!-- Verification Data -->
        <div class="footer-col legal-data">
          <h4>Información Comercial y Tributaria (RUC)</h4>
          <div class="data-grid">
            <div class="data-item">
              <span class="label">Propietario / Contribuyente</span>
              <span class="value">CARLOS ALFREDO LOPEZ PATIÑO</span>
            </div>
            <div class="data-item">
              <span class="label">RUC</span>
              <span class="value">0918539750001</span>
            </div>
            <div class="data-item">
              <span class="label">Estado RUC</span>
              <span class="value">ACTIVO</span>
            </div>
            <div class="data-item">
              <span class="label">Régimen / Tipo</span>
              <span class="value">GENERAL / Persona Natural</span>
            </div>
            <div class="data-item">
              <span class="label">Obligado a Llevar Contabilidad</span>
              <span class="value">NO</span>
            </div>
            <div class="data-item">
              <span class="label">Sucursales</span>
              <span class="value">2 Abiertas / 1 Cerrada</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Fechas SRI</span>
              <span class="value">Registro/Inicio: 28/08/2007 | Última Actualización: 08/06/2026</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Certificación RUC</span>
              <span class="value">Emisión: 08/06/2026 | Código de Verificación: RCR178093671013762</span>
            </div>
          </div>

          <h4 style="margin-top: 2rem; margin-bottom: 1rem;">Datos de Identidad y Filial</h4>
          <div class="data-grid">
            <div class="data-item">
              <span class="label">Cédula de Identidad (NUI)</span>
              <span class="value">091853975-0</span>
            </div>
            <div class="data-item">
              <span class="label">Nacionalidad / Sexo</span>
              <span class="value">Ecuatoriana / Hombre</span>
            </div>
            <div class="data-item">
              <span class="label">Fecha de Nacimiento</span>
              <span class="value">24 de septiembre de 1986</span>
            </div>
            <div class="data-item">
              <span class="label">Estado Civil</span>
              <span class="value">Casado con Alexandra Margarita Vascones Pita</span>
            </div>
            <div class="data-item">
              <span class="label">Nivel de Instrucción</span>
              <span class="value">Superior (Magíster)</span>
            </div>
            <div class="data-item">
              <span class="label">Emisión Cédula</span>
              <span class="value">Guayaquil, 11/02/2021 (Expira: 11/02/2031)</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Filiación de Padres</span>
              <span class="value">Padre: Carlos Armando Lopez Landin <br/> Madre: Elsa Cecilia Gladys Patiño Nuñez</span>
            </div>
          </div>

          <h4 style="margin-top: 2rem; margin-bottom: 1rem;">Actividades Económicas Autorizadas</h4>
          <div class="activities-list">
            <div class="activity-group">
              <h5>Servicios de Alimentación</h5>
              <p>Venta de comidas y bebidas en restaurantes, cafeterías, locales de comida rápida, heladerías y fuentes de soda.</p>
            </div>
            <div class="activity-group">
              <h5>Tecnología e Informática</h5>
              <p>Diseño de estructura, contenido y escritura de código (programas, aplicaciones web y bases de datos).</p>
            </div>
            <div class="activity-group">
              <h5>Producción Audiovisual</h5>
              <p>Producción cinematográfica, videos, anuncios de TV, edición de audio, fotografía comercial y prensa.</p>
            </div>
            <div class="activity-group">
              <h5>Actividades Inmobiliarias</h5>
              <p>Alquiler de bienes inmuebles a cambio de una retribución o por contrato (locales comerciales).</p>
            </div>
          </div>
        </div>

        <!-- Address -->
        <div class="footer-col address-col">
          <h4>Ubicación</h4>
          <p>
            Provincia: Guayas<br>
            Cantón: Guayaquil<br>
            Parroquia: Tarqui<br>
            Calle Avenida Circunvalación,<br>
            Manzana 25, Solar 16, entre 3era y 7ma<br>
            <strong>Referencia:</strong> Diagonal a la Iglesia Evangélica Bautista<br>
            Ecuador
          </p>
          <div class="tax-badges">
            <span class="badge">RUC Activo</span>
            <span class="badge">Régimen General</span>
            <span class="badge">Servicios Turísticos</span>
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
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=Inter:wght@300;400;500&display=swap');

$font-display: 'Syne', sans-serif;
$font-body: 'Inter', sans-serif;
$color-bg: #0d0b0a;
$color-text: #fcf8f2;
$color-accent: #dfa841;
$color-muted: #a69c90;
$color-green: #4a5d4e;
$color-red: #8f3d30;

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
      aspect-ratio: 4 / 3;

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
  background: #090807;
  padding: 6rem 4rem 2rem;
  border-top: 1px solid rgba(255,255,255,0.05);

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
            border-color: rgba(255, 255, 255, 0.5);
            color: #fff;
            background: rgba(255, 255, 255, 0.05);
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
            color: #7a6e60;
          }
          .value {
            font-size: 0.85rem;
            color: #ddd;
          }
        }
      }

      .activities-list {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 1.5rem;
        margin-top: 1rem;

        .activity-group {
          h5 {
            font-family: $font-display;
            font-size: 0.9rem;
            color: $color-accent;
            margin: 0 0 0.35rem 0;
            font-weight: 700;
          }
          p {
            font-size: 0.8rem;
            color: #bbb;
            line-height: 1.4;
            margin: 0;
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
      &.large, &.wide, &:not(.large):not(.wide) {
        grid-column: span 12;
        margin-top: 0;
        aspect-ratio: 16 / 10;
      }
    }
  }
}
@media (max-width: 768px) {
  .legal-footer .legal-data {
    .data-grid {
      grid-template-columns: 1fr;
      .span-2 {
        grid-column: span 1;
      }
    }
    .activities-list {
      grid-template-columns: 1fr;
    }
  }
}
</style>
