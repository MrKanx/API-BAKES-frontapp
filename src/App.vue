<script setup lang="ts">
import { ref, computed } from 'vue'

// Estado del menú
const selectedCategory = ref<'all' | 'cookies' | 'brownies' | 'pastry'>('all')

const categories = [
  { id: 'all', name: 'Todos los Postres' },
  { id: 'cookies', name: 'Galletas (Cookies)' },
  { id: 'brownies', name: 'Brownies & Cuchareables' },
  { id: 'pastry', name: 'Pastelería & Eventos' }
]

const menuItems = [
  {
    id: 1,
    category: 'cookies',
    name: 'Galletones New York Style',
    description: 'Galletas de tamaño grande, estilo New York, crujientes por fuera y súper gorditas y suaves por dentro.',
    tags: ['NYC Style', 'Artesanal'],
    price: 'Favorito',
    image: '/images/api_bakes_cookies.png'
  },
  {
    id: 2,
    category: 'cookies',
    name: 'Galletas Rellenas Especiales',
    description: 'Nuestra especialidad absoluta. Con rellenos ultra generosos. Los sabores más aclamados son Nutella y Leche Nido.',
    tags: ['Relleno Generoso', 'Especialidad'],
    price: 'Premium',
    image: '/images/api_bakes_cookies.png'
  },
  {
    id: 3,
    category: 'cookies',
    name: 'Cookie & Brownie Bites',
    description: 'Versiones miniatura de nuestras galletas y brownies. Se venden por docenas o en cajas especiales de 36 o 40 unidades.',
    tags: ['Para Compartir', 'Bites'],
    price: 'Por Cajas',
    image: '/images/api_bakes_hero.png'
  },
  {
    id: 4,
    category: 'cookies',
    name: 'Api Fries',
    description: 'Divertidas tiras de masa de galleta recién horneadas con forma de "papas fritas". Servidas con deliciosos dips de Nutella o Manjar.',
    tags: ['Original', 'Con Dips'],
    price: 'Divertido',
    image: '/images/api_bakes_hero.png'
  },
  {
    id: 5,
    category: 'brownies',
    name: 'Brownies Fudgy (Negritos)',
    description: 'Textura fudgy perfecta: húmedos, densos y cargados de chocolate. Olvídate del estilo bizcocho común, esto es chocolate real.',
    tags: ['Fudgy', 'Cacao Puro'],
    price: 'Irresistible',
    image: '/images/api_bakes_brownies.png'
  },
  {
    id: 6,
    category: 'brownies',
    name: 'Postres Cuchareables',
    description: 'Tarrinas gourmet diseñadas para devorar directo con cuchara. Capas perfectas. Ejemplo: Oreo & Nutella con mucho chocolate y trozos crujientes.',
    tags: ['Cuchareable', 'Oreo & Nutella'],
    price: 'En Tarrina',
    image: '/images/api_bakes_desserts.png'
  },
  {
    id: 7,
    category: 'pastry',
    name: 'Artisanal Cupcakes',
    description: 'Esponjosos cupcakes horneados en lotes pequeños y coronados con nuestro sedoso buttercream artesanal hecho desde cero.',
    tags: ['Buttercream', 'Decorados'],
    price: 'Bajo Pedido',
    image: '/images/api_bakes_desserts.png'
  },
  {
    id: 8,
    category: 'pastry',
    name: 'Brazo Gitano Artesanal',
    description: 'Bizcocho enrollado súper suave relleno de dulce tradicional. Disponible en tamaño MINI (ideal antojo) y Familiar.',
    tags: ['Clásico', 'Familiar o Mini'],
    price: 'Tradicional',
    image: '/images/api_bakes_hero.png'
  },
  {
    id: 9,
    category: 'pastry',
    name: 'Kits de Regalo (Cookie Boxes)',
    description: 'Cajas de galletas de temporada decoradas y personalizadas para fechas especiales: Día del Padre, San Valentín o Navidad.',
    tags: ['Personalizado', 'Regalo Especial'],
    price: 'Kits de Temporada',
    image: '/images/api_bakes_hero.png'
  }
]

const filteredItems = computed(() => {
  if (selectedCategory.value === 'all') return menuItems
  return menuItems.filter(item => item.category === selectedCategory.value)
})
</script>

<template>
  <div class="smooth-scroll-wrapper">
    <!-- HEADER / HERO -->
    <header class="hero">
      <div class="hero-bg" style="background-image: url('/images/api_bakes_hero.png');"></div>
      <div class="hero-overlay"></div>
      
      <nav class="nav">
        <div class="logo">API BAKES</div>
        <a href="#contacto" class="btn-contact">Contacto</a>
      </nav>

      <div class="hero-content">
        <div class="reveal-text">
          <h1 class="display-title">API <br/> BAKES</h1>
        </div>
        <p class="hero-subtitle">
          Repostería artesanal horneada en lotes pequeños bajo pedido en Samborondón, Ecuador. 
          Postres hechos a mano con un enfoque en texturas indulgentes y personalización para eventos o regalos.
        </p>
      </div>

      <div class="scroll-indicator">
        <div class="mouse"></div>
        <span>Desliza para ver</span>
      </div>
    </header>

    <!-- MARQUEE -->
    <div class="marquee-container">
      <div class="marquee">
        <span>GALLETAS &mdash; BROWNIES &mdash; CUCHAREABLES &mdash; CUPCAKES &mdash; BRAZO GITANO &mdash; PACKS DE REGALO &mdash; HECHO BAJO PEDIDO &mdash; </span>
        <span>GALLETAS &mdash; BROWNIES &mdash; CUCHAREABLES &mdash; CUPCAKES &mdash; BRAZO GITANO &mdash; PACKS DE REGALO &mdash; HECHO BAJO PEDIDO &mdash; </span>
      </div>
    </div>

    <!-- SECCIÓN NUESTRA PROPUESTA -->
    <section id="filosofia" class="gallery">
      <div class="gallery-header">
        <h2 class="section-title">NUESTRA <br/> PROPUESTA</h2>
        <p class="section-desc">
          Nos especializamos en postres reconfortantes (Comfort Desserts) modernos, horneados en casa bajo pedido. 
          "Detrás de cada pedido hay una historia", por lo que cuidamos cada detalle para garantizar frescura y un sabor casero auténtico.
        </p>
      </div>

      <div class="gallery-grid">
        <div class="gallery-item large">
          <div class="image-wrapper">
            <img src="/images/api_bakes_cookies.png" alt="Galletones y Galletas Rellenas" />
            <div class="item-overlay">
              <h3>Galletas Rellenas & Galletones</h3>
              <p>Galletas de tamaño grande estilo New York, crujientes y rellenas de Nutella o Leche Nido.</p>
            </div>
          </div>
        </div>
        <div class="gallery-item">
          <div class="image-wrapper">
            <img src="/images/api_bakes_brownies.png" alt="Brownies Fudgy" />
            <div class="item-overlay">
              <h3>Brownies (Negritos)</h3>
              <p>Textura fudgy, húmeda y densa. Cacao puro horneado con pasión.</p>
            </div>
          </div>
        </div>
        <div class="gallery-item wide">
          <div class="image-wrapper">
            <img src="/images/api_bakes_desserts.png" alt="Postres Cuchareables y Cupcakes" />
            <div class="item-overlay">
              <h3>Cuchareables & Cupcakes</h3>
              <p>Tarrinas gourmet de Oreo & Nutella y cupcakes decorados con buttercream artesanal.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- SECCIÓN MENÚ / CATÁLOGO -->
    <section id="menu" class="menu-section">
      <div class="menu-header">
        <h2 class="section-title">NUESTRO MENÚ</h2>
        <p class="section-desc">Selecciona una categoría para ver nuestras especialidades horneadas bajo pedido.</p>
        
        <div class="filter-tabs">
          <button 
            v-for="cat in categories" 
            :key="cat.id"
            :class="['filter-btn', { active: selectedCategory === cat.id }]"
            @click="selectedCategory = cat.id as any"
          >
            {{ cat.name }}
          </button>
        </div>
      </div>

      <!-- Grid de Postres -->
      <div class="menu-grid">
        <div v-for="item in filteredItems" :key="item.id" class="menu-card">
          <div class="card-img-wrapper">
            <img :src="item.image" :alt="item.name" />
            <div class="card-tag">{{ item.price }}</div>
          </div>
          <div class="card-content">
            <div class="card-header">
              <h3>{{ item.name }}</h3>
            </div>
            <p>{{ item.description }}</p>
            <div class="card-footer">
              <div class="tags-container">
                <span v-for="tag in item.tags" :key="tag" class="tag">{{ tag }}</span>
              </div>
              <a href="https://wa.me/593985284807" target="_blank" class="btn-order-item">Pedir</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- FOOTER (CON TODA LA INFORMACIÓN DE VERIFICACIÓN AL ESTILO DEL SITIO ORIGINAL) -->
    <footer id="contacto" class="legal-footer">
      <div class="footer-grid">
        <!-- Branding / Contact -->
        <div class="footer-col brand-col">
          <h2 class="footer-logo">API BAKES</h2>
          <p class="contact-email">
            <a href="mailto:anapaulaschweitzer29@gmail.com">anapaulaschweitzer29@gmail.com</a>
          </p>
          <div class="phones">
            <a href="tel:0985284807">0985284807</a>
          </div>
          <p class="copyright">&copy; 2026 SCHWEITZER VINTIMILLA ANA PAULA. Todos los derechos reservados.</p>
        </div>

        <!-- Verification Summary Quick -->
        <div class="footer-col legal-data">
          <h4>Resumen de Negocio</h4>
          <div class="data-grid">
            <div class="data-item">
              <span class="label">Propietario</span>
              <span class="value">SCHWEITZER VINTIMILLA ANA PAULA</span>
            </div>
            <div class="data-item">
              <span class="label">RUC</span>
              <span class="value">0922854674001</span>
            </div>
            <div class="data-item">
              <span class="label">Cédula (NUI)</span>
              <span class="value">0922854674</span>
            </div>
            <div class="data-item">
              <span class="label">Régimen</span>
              <span class="value">GENERAL</span>
            </div>
            <div class="data-item">
              <span class="label">Obligado Contabilidad</span>
              <span class="value">NO</span>
            </div>
            <div class="data-item">
              <span class="label">Estado RUC</span>
              <span class="value">ACTIVO</span>
            </div>
            <div class="data-item">
              <span class="label">Inicio Actividades</span>
              <span class="value">23/06/2020</span>
            </div>
            <div class="data-item">
              <span class="label">Última Actualización</span>
              <span class="value">11/12/2025</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Actividades Económicas SRI</span>
              <span class="value">
                • <strong>Alimenticias:</strong> Elaboración de tortas, tartas, etc. (API BAKES).<br>
                • <strong>Jurídicas:</strong> Asesoramiento civil, penal, laboral y prestación de servicios profesionales.<br>
                • <strong>Comerciales:</strong> Asesoramiento corporativo (cabildeo/lobbies) y servicios diversos.<br>
                • <strong>Agrícolas:</strong> Cultivos de frutos (pitahaya, tuna, algarropa, taxos, etc.).
              </span>
            </div>
            <div class="data-item span-2">
              <span class="label">Código Certificado RUC</span>
              <span class="value">RCR1777913868338118 (Emisión: 04/May/2026 - Verificable SRI en Línea, Res. NAC-DGERCGC15-00000217)</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Cédula Digital (Gob.EC)</span>
              <span class="value">No: 086030110 (Vence: 03/Jun/2032, Generado: 17/07/2026 10:45:58, Verificación QR y PIN pág. 3)</span>
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
            Dirección: Calle Av. José Joaquín Orrantia No. 801 e Intersección Av. Las Américas (Barrio: Calle General).<br>
            <strong>Referencia:</strong> Al lado de Grilling.<br>
            <strong>Establecimientos:</strong> 1 Abierto / 0 Cerrados<br>
            <strong>Nacionalidad:</strong> Ecuatoriana (Nacimiento: 29 de mayo de 2000)<br>
            <strong>Estado Civil:</strong> Casada (Cónyuge: Juan Javier Neira Anda)
          </p>
          <div class="tax-badges">
            <span class="badge">RUC Activo</span>
            <span class="badge">Régimen General</span>
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
$color-bg: #1c0e07; // Chocolate Profundo
$color-card: #2a1910; // Chocolate Café
$color-text: #faf6f0; // Crema Suave
$color-accent: #d4a373; // Oro Caramelo
$color-secondary: #e07a5f; // Sweet Coral / Baya
$color-muted: #a3958c; // Muted Cocoa Gray

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
        color: $color-bg;
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
  background: #140903;
  border-top: 1px solid rgba($color-accent, 0.15);
  border-bottom: 1px solid rgba($color-accent, 0.15);
  color: #fff;
  overflow: hidden;
  white-space: nowrap;
  box-shadow: 0 0 20px rgba($color-accent, 0.03);

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
      max-width: 450px;
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
        border-color: rgba($color-accent, 0.3);
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

/* MENU SECTION */
.menu-section {
  padding: 6rem 4rem 10vw;
  border-top: 1px solid rgba($color-accent, 0.1);

  .menu-header {
    text-align: center;
    max-width: 800px;
    margin: 0 auto 5rem;

    .section-title {
      font-family: $font-display;
      font-size: clamp(2.5rem, 5vw, 4rem);
      margin: 0 0 1rem;
      font-weight: 800;
    }

    .section-desc {
      color: $color-muted;
      font-size: 1.1rem;
      margin-bottom: 3rem;
    }

    .filter-tabs {
      display: inline-flex;
      background: rgba($color-card, 0.5);
      border: 1px solid rgba($color-accent, 0.15);
      padding: 0.4rem;
      border-radius: 50px;
      flex-wrap: wrap;
      justify-content: center;
      gap: 0.2rem;

      .filter-btn {
        background: transparent;
        border: none;
        color: $color-muted;
        font-family: $font-body;
        font-size: 0.9rem;
        font-weight: 500;
        padding: 0.8rem 1.6rem;
        border-radius: 50px;
        cursor: pointer;
        transition: all 0.3s ease;

        &.active, &:hover {
          background-color: $color-accent;
          color: $color-bg;
          font-weight: 700;
        }
      }
    }
  }

  .menu-grid {
    max-width: 1200px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2.5rem;

    .menu-card {
      background-color: $color-card;
      border-radius: 18px;
      overflow: hidden;
      border: 1px solid rgba($color-accent, 0.08);
      transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
      display: flex;
      flex-direction: column;

      &:hover {
        transform: translateY(-8px);
        border-color: rgba($color-accent, 0.3);
        box-shadow: 0 20px 40px rgba(0,0,0,0.4);

        .card-img-wrapper img {
          transform: scale(1.05);
        }
      }

      .card-img-wrapper {
        position: relative;
        aspect-ratio: 16 / 11;
        overflow: hidden;
        background-color: #0c0502;

        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          transition: transform 0.6s ease;
        }

        .card-tag {
          position: absolute;
          top: 1rem;
          right: 1rem;
          background: rgba($color-bg, 0.85);
          color: $color-accent;
          font-size: 0.75rem;
          font-weight: 700;
          letter-spacing: 0.05em;
          padding: 0.4rem 0.9rem;
          border-radius: 50px;
          border: 1px solid rgba($color-accent, 0.25);
          backdrop-filter: blur(5px);
        }
      }

      .card-content {
        padding: 2rem;
        display: flex;
        flex-direction: column;
        flex-grow: 1;

        .card-header {
          margin-bottom: 0.8rem;
          
          h3 {
            font-family: $font-display;
            font-size: 1.45rem;
            font-weight: 700;
            margin: 0;
            color: $color-text;
            line-height: 1.25;
          }
        }

        p {
          color: $color-muted;
          font-size: 0.92rem;
          line-height: 1.5;
          margin: 0 0 2rem;
          flex-grow: 1;
        }

        .card-footer {
          display: flex;
          justify-content: space-between;
          align-items: center;
          margin-top: auto;
          gap: 1rem;

          .tags-container {
            display: flex;
            gap: 0.4rem;
            flex-wrap: wrap;

            .tag {
              font-size: 0.7rem;
              background-color: rgba($color-accent, 0.06);
              color: $color-accent;
              padding: 0.25rem 0.6rem;
              border-radius: 4px;
              border: 1px solid rgba($color-accent, 0.12);
            }
          }

          .btn-order-item {
            background-color: transparent;
            border: 1px solid rgba($color-accent, 0.3);
            color: $color-accent;
            text-decoration: none;
            font-size: 0.8rem;
            font-weight: 700;
            padding: 0.45rem 1.1rem;
            border-radius: 50px;
            transition: all 0.3s ease;

            &:hover {
              background-color: $color-accent;
              color: $color-bg;
              border-color: $color-accent;
            }
          }
        }
      }
    }
  }
}

/* FOOTER */
.legal-footer {
  background: #0f0704;
  padding: 6rem 4rem 2rem;
  border-top: 1px solid rgba($color-accent, 0.15);

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
          color: $color-accent;
          font-weight: 700;
        }
      }
      .copyright {
        margin-top: 3rem;
        font-size: 0.75rem;
        opacity: 0.5;
        line-height: 1.4;
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
          border: 1px solid rgba($color-accent, 0.25);
          border-radius: 4px;
          color: $color-muted;
          text-transform: uppercase;
          letter-spacing: 0.05em;
          transition: all 0.3s ease;
          cursor: default;

          &:hover {
            border-color: $color-accent;
            color: #fff;
            background: rgba($color-accent, 0.05);
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
            line-height: 1.4;
          }
        }
      }
    }
  }

  .footer-bottom {
    margin-top: 3rem;
    padding-top: 1.5rem;
    border-top: 1px solid rgba($color-accent, 0.1);
    text-align: center;

    .developer-credit {
      font-size: 0.8rem;
      color: #615249;
      letter-spacing: 0.05em;

      a {
        color: #8c786b;
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
  .menu-section { padding: 6rem 2rem; }
  
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

  .menu-section .menu-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 768px) {
  .menu-section .menu-grid {
    grid-template-columns: 1fr;
  }
}
</style>
