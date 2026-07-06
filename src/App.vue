<script setup lang="ts">
import { ref } from 'vue'

const activeTab = ref('identificacion')
</script>

<template>
  <div class="smooth-scroll-wrapper">
    <!-- HERO SECTION -->
    <section class="hero">
      <div class="hero-bg" style="background-image: url('/images/ohayo_hero_bg.png');"></div>
      <div class="hero-overlay"></div>
      
      <nav class="nav">
        <div class="logo">OHAYO ECUADOR</div>
        <a href="#verificacion" class="btn-contact">Verificación Comercial</a>
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

    <!-- PORTFOLIO / VERIFICATION DASHBOARD -->
    <section id="verificacion" class="verification">
      <div class="verification-header">
        <h2 class="section-title">PORTAFOLIO <br/> COMERCIAL</h2>
        <p class="section-desc">Aquí tienes recopilados y organizados todos los datos clave extraídos de los documentos oficiales de <strong>Brandon Santiago Coello Moreira</strong>, listos para verificación.</p>
      </div>

      <div class="dashboard-container">
        <!-- Tabs Nav -->
        <div class="dashboard-tabs">
          <button 
            :class="['tab-btn', { active: activeTab === 'identificacion' }]"
            @click="activeTab = 'identificacion'"
          >
            <span class="icon">👤</span> Identificación Personal
          </button>
          <button 
            :class="['tab-btn', { active: activeTab === 'tributaria' }]"
            @click="activeTab = 'tributaria'"
          >
            <span class="icon">💼</span> Información Tributaria (RUC)
          </button>
          <button 
            :class="['tab-btn', { active: activeTab === 'financiera' }]"
            @click="activeTab = 'financiera'"
          >
            <span class="icon">🏦</span> Información Financiera
          </button>
        </div>

        <!-- Tab Panels -->
        <div class="dashboard-content">
          <!-- Tab 1: Identificación -->
          <div v-if="activeTab === 'identificacion'" class="tab-panel fade-in">
            <div class="profile-card">
              <div class="profile-header">
                <div class="profile-avatar">BS</div>
                <div class="profile-title">
                  <h3>COELLO MOREIRA BRANDON SANTIAGO</h3>
                  <span class="profile-status">Instrucción: Superior / Estudiante</span>
                </div>
              </div>
              
              <div class="profile-grid">
                <div class="info-group">
                  <span class="info-label">Cédula de Ciudadanía</span>
                  <span class="info-value">095226552-8</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Nacionalidad</span>
                  <span class="info-value">Ecuatoriana</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Fecha de Nacimiento</span>
                  <span class="info-value">4 de enero de 1995</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Sexo</span>
                  <span class="info-value">Hombre</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Estado Civil</span>
                  <span class="info-value">Soltero</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Datos Familiares (Padres)</span>
                  <span class="info-value">
                    <strong>Padre:</strong> Coello Bustamante Ledo Humberto <br>
                    <strong>Madre:</strong> Moreira Villacres Tania Elizabeth
                  </span>
                </div>
                <div class="info-group span-2">
                  <span class="info-label">Detalles del Documento de Identidad</span>
                  <span class="info-value">
                    Expedido en la ciudad de <strong>Guayaquil</strong> el 15 de octubre de 2018. <br>
                    Fecha de expiración: 15 de octubre de 2028.
                  </span>
                </div>
              </div>
            </div>
          </div>

          <!-- Tab 2: Información Tributaria -->
          <div v-if="activeTab === 'tributaria'" class="tab-panel fade-in">
            <div class="ruc-card">
              <div class="ruc-header">
                <div>
                  <span class="ruc-title">Registro Único de Contribuyentes (SRI)</span>
                  <h3>RUC: 0952265528001</h3>
                </div>
                <span class="status-badge active">RUC Activo</span>
              </div>
              
              <div class="ruc-grid">
                <div class="info-group">
                  <span class="info-label">Régimen Impositivo</span>
                  <span class="info-value text-highlight">RIMPE - Negocio Popular</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Inicio de Actividades</span>
                  <span class="info-value">7 de febrero de 2024</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Obligado a llevar contabilidad</span>
                  <span class="info-value">No</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Condiciones Especiales</span>
                  <span class="info-value">Artesano: No | Contribuyente Especial: No | Agente de Retención: No</span>
                </div>
                <div class="info-group span-2">
                  <span class="info-label">Actividad Económica Principal</span>
                  <span class="info-value text-highlight">G46900002 - Venta al por mayor de otros productos diversos para el consumidor.</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Establecimientos registrados</span>
                  <span class="info-value">1 Abierto / 0 Cerrados</span>
                </div>
                <div class="info-group">
                  <span class="info-label">Obligaciones Tributarias</span>
                  <span class="info-value">1011 Declaración de Impuesto a la Renta Personas Naturales.</span>
                </div>
                
                <div class="info-group span-2 address-detail">
                  <span class="info-label">Domicilio Tributario</span>
                  <span class="info-value">
                    <strong>Ubicación:</strong> Provincia: Guayas, Cantón: Guayaquil, Parroquia: Tarqui. <br>
                    <strong>Dirección:</strong> Barrio Garzota 2, Calle Washington Delgado C., Número: Villa 8, Intersección: 14 Pasaje 3 NE. <br>
                    <strong>Referencia:</strong> A una cuadra del gimnasio Vikingos.
                  </span>
                </div>

                <div class="info-group">
                  <span class="info-label">Email de Contacto RUC</span>
                  <span class="info-value"><a href="mailto:brandoncoellomoreira@gmail.com">brandoncoellomoreira@gmail.com</a></span>
                </div>
                <div class="info-group">
                  <span class="info-label">Celular de Contacto RUC</span>
                  <span class="info-value"><a href="tel:0995076954">0995076954</a></span>
                </div>

                <div class="info-group span-2 certification-box">
                  <span class="info-label">Datos de Emisión del Certificado RUC</span>
                  <span class="info-value">
                    Código de validación <strong>RCR1781740466673260</strong>, emitido por el SRI el 17 de junio de 2026 a las 18:54.
                  </span>
                </div>
              </div>
            </div>
          </div>

          <!-- Tab 3: Información Financiera -->
          <div v-if="activeTab === 'financiera'" class="tab-panel fade-in">
            <div class="finance-card">
              <div class="finance-header">
                <div>
                  <span class="finance-title">Certificado Bancario Produbanco</span>
                  <h3>Cuentas Bancarias Activas (en Dólares USA)</h3>
                </div>
                <span class="status-badge date">Vigente hasta: 21/Jul/2026</span>
              </div>

              <div class="table-responsive">
                <table class="finance-table">
                  <thead>
                    <tr>
                      <th>Tipo de Cuenta</th>
                      <th>Número de Cuenta</th>
                      <th>Fecha de Apertura</th>
                      <th>Saldo Promedio Semestral</th>
                      <th>Estado</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <td class="account-name">Cuenta BE</td>
                      <td>18001326761</td>
                      <td>2024/04/02</td>
                      <td class="balance">$123.24</td>
                      <td><span class="badge-success">Activa</span></td>
                    </tr>
                    <tr>
                      <td class="account-name">Cuenta Digital</td>
                      <td>20006594921</td>
                      <td>2025/11/13</td>
                      <td class="balance">$17.55</td>
                      <td><span class="badge-success">Activa</span></td>
                    </tr>
                    <tr>
                      <td class="account-name">Ahorro a tu Gusto</td>
                      <td>16000622931</td>
                      <td>2026/03/11</td>
                      <td class="balance">$8.27</td>
                      <td><span class="badge-success">Activa</span></td>
                    </tr>
                    <tr>
                      <td class="account-name">Flexiahorro</td>
                      <td>28002464504</td>
                      <td>2026/03/11</td>
                      <td class="balance">$0.00</td>
                      <td><span class="badge-success">Activa</span></td>
                    </tr>
                  </tbody>
                </table>
              </div>

              <div class="finance-notes">
                <p><strong>Nota importante:</strong> Todas las cuentas figuran en estado <strong>Activa</strong> y sin ningún tipo de protestos en el sistema financiero.</p>
                
                <div class="extra-indicators">
                  <div class="indicator-item">
                    <span class="indicator-label">Inversiones</span>
                    <span class="indicator-value negative">No mantiene inversiones con el banco.</span>
                  </div>
                  <div class="indicator-item">
                    <span class="indicator-label">Riesgos</span>
                    <span class="indicator-value negative">No mantiene riesgos con el banco.</span>
                  </div>
                </div>
              </div>
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

/* PORTFOLIO / VERIFICATION DASHBOARD */
.verification {
  padding: 8vw 4rem;
  background: darken($color-bg, 1.5%);
  border-top: 1px solid rgba(255, 255, 255, 0.03);

  .verification-header {
    margin-bottom: 4rem;
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
      text-transform: uppercase;
    }

    .section-desc {
      max-width: 450px;
      font-size: 1.1rem;
      color: $color-muted;
      line-height: 1.6;
    }
  }

  .dashboard-container {
    background: $color-card;
    border: 1px solid rgba(255, 255, 255, 0.05);
    border-radius: 16px;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.5);
    backdrop-filter: blur(10px);
  }

  .dashboard-tabs {
    display: flex;
    border-bottom: 1px solid rgba(255, 255, 255, 0.05);
    background: rgba(0, 0, 0, 0.2);

    .tab-btn {
      flex: 1;
      background: transparent;
      border: none;
      color: $color-muted;
      padding: 1.5rem;
      font-family: $font-display;
      font-size: 1.1rem;
      font-weight: 700;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 0.75rem;
      transition: all 0.3s ease;
      border-bottom: 2px solid transparent;

      .icon {
        font-size: 1.2rem;
        filter: grayscale(1);
        transition: filter 0.3s ease;
      }

      &:hover {
        color: #fff;
        background: rgba(255, 255, 255, 0.02);
      }

      &.active {
        color: $color-secondary;
        border-bottom-color: $color-secondary;
        background: rgba(255, 255, 255, 0.01);

        .icon {
          filter: grayscale(0);
        }
      }
    }
  }

  .dashboard-content {
    padding: 3rem;

    .fade-in {
      animation: fadeIn 0.5s ease forwards;
    }
  }

  /* Profile Card Details */
  .profile-card, .ruc-card, .finance-card {
    display: flex;
    flex-direction: column;
    gap: 2.5rem;
  }

  .profile-header, .ruc-header, .finance-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid rgba(255, 255, 255, 0.05);
    padding-bottom: 1.5rem;
    flex-wrap: wrap;
    gap: 1rem;

    h3 {
      font-family: $font-display;
      font-size: 1.8rem;
      margin: 0.25rem 0 0;
      color: #fff;
      letter-spacing: -0.01em;
    }

    .profile-avatar {
      width: 60px;
      height: 60px;
      background: linear-gradient(135deg, $color-accent, $color-secondary);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: $font-display;
      font-weight: 800;
      font-size: 1.5rem;
      color: #fff;
      box-shadow: 0 0 15px rgba($color-accent, 0.3);
    }

    .profile-title {
      display: flex;
      flex-direction: column;
      
      .profile-status {
        font-size: 0.85rem;
        color: $color-secondary;
        text-transform: uppercase;
        letter-spacing: 0.05em;
      }
    }

    .ruc-title, .finance-title {
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: $color-muted;
    }

    .status-badge {
      padding: 0.5rem 1rem;
      border-radius: 50px;
      font-size: 0.8rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.05em;

      &.active {
        background: rgba(0, 229, 255, 0.1);
        color: $color-secondary;
        border: 1px solid rgba(0, 229, 255, 0.2);
        box-shadow: 0 0 10px rgba($color-secondary, 0.1);
      }

      &.date {
        background: rgba(255, 42, 95, 0.1);
        color: $color-accent;
        border: 1px solid rgba(255, 42, 95, 0.2);
      }
    }
  }

  .profile-grid, .ruc-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;

    .info-group {
      display: flex;
      flex-direction: column;
      gap: 0.4rem;

      &.span-2 {
        grid-column: span 2;
      }

      .info-label {
        font-size: 0.75rem;
        text-transform: uppercase;
        letter-spacing: 0.05em;
        color: $color-muted;
      }

      .info-value {
        font-size: 1.05rem;
        color: #ddd;
        line-height: 1.6;

        a {
          color: $color-secondary;
          text-decoration: none;
          transition: color 0.3s;
          &:hover {
            color: #fff;
            text-decoration: underline;
          }
        }

        strong {
          color: #fff;
        }

        &.text-highlight {
          color: $color-accent;
          font-weight: 700;
        }
      }
    }

    .address-detail {
      background: rgba(0, 0, 0, 0.15);
      padding: 1.5rem;
      border-radius: 8px;
      border-left: 3px solid $color-secondary;
    }

    .certification-box {
      background: rgba(255, 42, 95, 0.05);
      padding: 1.25rem 1.5rem;
      border-radius: 8px;
      border-left: 3px solid $color-accent;
      margin-top: 1rem;
    }
  }

  /* Table styling */
  .table-responsive {
    overflow-x: auto;
  }

  .finance-table {
    width: 100%;
    border-collapse: collapse;
    text-align: left;

    th {
      padding: 1.2rem 1.5rem;
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: $color-muted;
      border-bottom: 1px solid rgba(255, 255, 255, 0.08);
      font-weight: 500;
    }

    td {
      padding: 1.2rem 1.5rem;
      font-size: 0.95rem;
      color: #ddd;
      border-bottom: 1px solid rgba(255, 255, 255, 0.04);
      transition: all 0.3s ease;

      &.account-name {
        font-family: $font-display;
        font-weight: 700;
        color: #fff;
      }

      &.balance {
        font-family: monospace;
        font-weight: 700;
        color: $color-secondary;
        font-size: 1.05rem;
      }

      .badge-success {
        background: rgba(0, 229, 255, 0.1);
        color: $color-secondary;
        padding: 0.25rem 0.6rem;
        border-radius: 4px;
        font-size: 0.75rem;
        font-weight: 700;
        text-transform: uppercase;
        border: 1px solid rgba(0, 229, 255, 0.15);
      }
    }

    tr:hover td {
      background: rgba(255, 255, 255, 0.01);
    }
  }

  .finance-notes {
    margin-top: 1.5rem;
    
    p {
      color: $color-muted;
      font-size: 0.9rem;
      margin-bottom: 2rem;
      
      strong {
        color: #ddd;
      }
    }

    .extra-indicators {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 2rem;

      .indicator-item {
        background: rgba(0, 0, 0, 0.15);
        padding: 1.5rem;
        border-radius: 8px;
        border: 1px solid rgba(255, 255, 255, 0.03);
        display: flex;
        flex-direction: column;
        gap: 0.4rem;

        .indicator-label {
          font-size: 0.75rem;
          text-transform: uppercase;
          letter-spacing: 0.05em;
          color: $color-muted;
        }

        .indicator-value {
          font-size: 0.95rem;
          color: #ddd;

          &.negative {
            color: $color-muted;
            font-style: italic;
          }
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
  .verification { padding: 6vw 2rem; }
  
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
  .verification {
    .dashboard-tabs {
      flex-direction: column;
      
      .tab-btn {
        padding: 1rem;
        border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        border-left: 2px solid transparent;
        justify-content: flex-start;
        
        &.active {
          border-bottom-color: transparent;
          border-left-color: $color-secondary;
        }
      }
    }
    
    .dashboard-content {
      padding: 1.5rem;
    }
    
    .profile-grid, .ruc-grid {
      grid-template-columns: 1fr;
      gap: 1.5rem;
      
      .info-group.span-2 {
        grid-column: span 1;
      }
    }
    
    .finance-notes {
      .extra-indicators {
        grid-template-columns: 1fr;
        gap: 1rem;
      }
    }
  }
}
</style>
