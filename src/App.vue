<script setup>

import { computed, ref } from 'vue'

const phone = '5214642217051'

const whatsappBase = `https://wa.me/${phone}`

const messageFor = (product) =>

  `${whatsappBase}?text=${encodeURIComponent(

    `Hola, vi su página web de Proyectos Modernos en Decoración y me interesa recibir información y una cotización de: ${product}.`

  )}`

const generalMessage = computed(() =>

  `${whatsappBase}?text=${encodeURIComponent(

    'Hola, vi la página de Proyectos Modernos en Decoración y me gustaría recibir información sobre sus productos y servicios.'

  )}`

)

const address = 'C. Morelos 1002, Centro, 36740 Salamanca, Guanajuato, México'

const mapLink = `https://www.google.com/maps/search/?api=1&query=${encodeURIComponent(address)}`

const socialLinks = [

  {

    name: 'Facebook',

    url: 'https://www.facebook.com/pmdbajio?mibextid=ZbWKwL',

    label: 'Síguenos en Facebook',

  },

  {

    name: 'Instagram',

    url: 'https://www.instagram.com/proyectosmodernosendecoracion?stkn=aWl1aXdhY2xuOWNx',

    label: 'Síguenos en Instagram',

  },

  {

    name: 'TikTok',

    url: 'https://www.tiktok.com/@proyectos.moderno?_r=1&_t=ZS-9AHLwJACPO1',

    label: 'Síguenos en TikTok',

  },

]

const categories = [

  {

    name: 'Persianas',

    description: 'Suministro, instalación, mantenimiento y reparación de persianas de PVC, Sheer Elegance y enrollables.',

    image: '/images/persiana1.png',

    gallery: [

      '/images/persiana1.png',

      '/images/persiana2.png',

      '/images/persiana3.png',

      '/images/persiana4.png',

      '/images/persiana5.png',

      '/images/persiana6.png',

      '/images/persiana7.png',

      '/images/persiana8.png',

      '/images/persiana9.png',

    ],

  },

  {

    name: 'Pisos vinílicos y laminados',

    description: 'Opciones para renovar tus espacios con pisos vinílicos, laminados y acabados modernos.',

    image: '/images/pisola1.png',

    gallery: [

      '/images/pisola1.png',

      '/images/pisola2.png',

      '/images/pisola3.png',

      '/images/pisola4.png',

      '/images/pisola5.png',

      '/images/pisola6.png',

    ],

  },

  {

    name: 'Cocinas y clósets',

    description: 'Muebles de melamina para cocinas integrales, clósets, centros de entretenimiento y mostradores.',

    image: '/images/cocinas-closets-01.png',

    gallery: [

      '/images/cocinas-closets-02.png',

      '/images/cocinas-closets-03.png',

      '/images/cocinas-closets-04.png',

      '/images/cocinas-closets-05.png',

      '/images/cocinas-closets-06.png',

      '/images/cocinas-closets-07.png',

      '/images/cocinas-closets-08.png',

      '/images/cocinas-closets-09.png',

      '/images/cocinas-closets-10.png',

    ],

  },

  {

    name: 'Lambrín y placas de PVC',

    description: 'Revestimientos para interiores y exteriores que ayudan a renovar paredes y darles una nueva apariencia.',

    image: '/images/lambrin-placas-01.png',

    gallery: [

      '/images/lambrin-placas-02.png',

      '/images/lambrin-placas-03.png',

      '/images/lambrin-placas-04.png',

      '/images/lambrin-placas-05.png',

      '/images/lambrin-placas-06.png',

      '/images/lambrin-placas-07.png',

      '/images/lambrin-placas-08.png',

      '/images/lambrin-placas-09.png',

      '/images/lambrin-placas-10.png',

      '/images/lambrin-placas-11.png',

    ],

  },

    {

    name: 'Tablaroca, Durock y plafones',

    description: 'Suministro e instalación de tablaroca, Durock, muros y plafones para diferentes espacios.',

    image: '/images/tabla1.png',

    gallery: [

      '/images/tabla1.png',

      '/images/tabla2.png',

      '/images/tabla3.png',

      '/images/tabla4.png',

      '/images/tabla5.png',

      '/images/tabla6.png',

      '/images/tabla7.png',

    ],

  },

  {

    name: 'Pasto sintético y follaje',

    description: 'Pasto sintético para interior y exterior, follaje sintético y soluciones decorativas.',

    image: '/images/to1.png',

    gallery: [

      '/images/to1.png',

      '/images/to2.png',

      '/images/to3.png',

      '/images/to4.png',

      '/images/to5.png',

      '/images/to6.png',

      '/images/to7.png',

      '/images/to8.png',

      '/images/to9.png',

      '/images/to10.png',

      '/images/to11.png',

      '/images/to12.png',

    ],

  },

    {

    name: 'Papel tapiz y tapices',

    description: 'Papel tapiz para dar personalidad a muros y renovar la decoración de tus espacios.',

    image: '/images/tapices1.png',

    gallery: [

      '/images/tapices1.png',

      '/images/tapices2.png',

      '/images/tapices3.png',

      '/images/tapices4.png',

      '/images/tapices5.png',

    ],

  },

    {

    name: 'Canceles de baño',

    description: 'Soluciones para complementar y renovar la apariencia de tu baño.',

    image: '/images/baño1.png',

    gallery: [

      '/images/baño1.png',

      '/images/baño2.png',

      '/images/baño3.png',

      '/images/baño4.png',

      '/images/baño5.png',

      '/images/baño6.png',

    ],

  },

]

const services = [

  'Suministro e instalación de tablaroca, Durock, muros y plafones.',

  'Suministro, instalación, mantenimiento y reparación de persianas de PVC, Sheer Elegance y enrollables.',

  'Pasto sintético para interior y exterior, follaje sintético, lambrín para interior y exterior, y muros de PVC.',

  'Papel tapiz.',

  'Lavado de salas, alfombras, tapetes y sillas.',

  'Pintura.',

  'Pisos vinílicos y laminados.',

  'Muebles de melamina: cocinas, clósets, centros de entretenimiento y mostradores.',

  'Instalación de piso conductivo.',

  'Servicio de lavado, pulido y encerado de pisos vinílicos.',

]

const finishes = [

  {

    name: 'Piso laminado',

    description: 'Conoce las opciones de acabados para piso laminado.',

    image: '/images/muestrariopiso1.png',

    gallery: [

      '/images/muestrariopiso1.png',

      '/images/muestrariopiso2.png',

      '/images/muestrariopiso3.png',

    ],

  },

  {

    name: 'Piso SPC',

    description: 'Consulta nuestro muestrario de piso SPC.',

    image: '/images/muestrariospc1.png',

    gallery: [

      '/images/muestrariospc1.png',

    ],

  },

  {

    name: 'Duelas vinílicas',

    description: 'Consulta el muestrario de duelas vinílicas.',

    image: '/images/muestrarioduelas1.png',

    gallery: [

      '/images/muestrarioduelas1.png',

    ],

  },

]

const menuOpen = ref(false)

const selectedGallery = ref(null)

const selectedImage = ref(null)

const openGallery = (item) => {

  selectedGallery.value = item

  selectedImage.value = null

}

const closeGallery = () => {

  selectedGallery.value = null

  selectedImage.value = null

}

const openImage = (image) => {

  selectedImage.value = image

}

const closeImage = () => {

  selectedImage.value = null

}

</script>

<template>

  <div class="site-wrapper">

    <header class="navbar">

      <a class="brand" href="#inicio" aria-label="Proyectos Modernos en Decoración, inicio" @click="menuOpen = false">

        <img class="brand-logo" src="/images/logop-negro-dorado.png" alt="Proyectos Modernos en Decoración" />

        <span class="brand-name">

          <strong>Proyectos Modernos</strong>

          <small>en Decoración</small>

        </span>

      </a>

      <button class="menu-toggle" type="button" :aria-expanded="menuOpen" aria-label="Abrir menú de navegación" @click="menuOpen = !menuOpen">

        <span></span><span></span><span></span>

      </button>

      <nav class="nav-links" :class="{ 'nav-links-open': menuOpen }">

        <a href="#inicio" @click="menuOpen = false">Inicio</a>

        <a href="#catalogo" @click="menuOpen = false">Productos</a>

        <a href="#servicios" @click="menuOpen = false">Servicios</a>

        <a href="#muestrarios" @click="menuOpen = false">Muestrarios</a>

        <a href="#ubicacion" @click="menuOpen = false">Ubicación</a>

        <a class="nav-contact" :href="generalMessage" target="_blank" rel="noopener noreferrer" @click="menuOpen = false">

          Cotizar por WhatsApp

        </a>

      </nav>

    </header>

    <main>

      <section id="inicio" class="hero">

        <div class="hero-overlay"></div>

        <div class="hero-content">

          <p class="eyebrow">DISEÑO · CALIDAD · ACABADOS</p>

          <h1>Transformamos tus espacios en lugares extraordinarios.</h1>

          <p class="hero-description">

            Productos y servicios de decoración para crear ambientes elegantes,

            confortables y modernos, adaptados a tu espacio.

          </p>

          <div class="hero-actions">

            <a class="button button-primary" href="#catalogo">Conoce nuestros productos</a>

            <a class="button button-outline" :href="generalMessage" target="_blank" rel="noopener noreferrer">

              Solicitar cotización

            </a>

          </div>

        </div>

        <a class="hero-scroll" href="#catalogo">DESCUBRE MÁS <span>↓</span></a>

      </section>

      <section class="intro-strip">

        <div>

          <span class="intro-number">32+</span>

          <span class="intro-label">años de experiencia en el Estado de México</span>

        </div>

        <div>

          <span class="intro-number">2+</span>

          <span class="intro-label">años de experiencia en Salamanca, Guanajuato</span>

        </div>

        <div>

          <span class="intro-number">PMD</span>

          <span class="intro-label">Soluciones para tus espacios</span>

        </div>

      </section>

      <section id="catalogo" class="section section-padding">

        <div class="section-heading">

          <p class="eyebrow">NUESTROS PRODUCTOS</p>

          <h2>Detalles que transforman cada espacio</h2>

          <p>

            Conoce algunas de nuestras soluciones de decoración, mobiliario,

            recubrimientos y acabados.

          </p>

        </div>

        <div class="category-grid">

          <article v-for="category in categories" :key="category.name" class="category-card">

            <div class="category-image">

              <img :src="category.image" :alt="category.name" loading="lazy" />

            </div>

            <div class="category-info">

              <h3>{{ category.name }}</h3>

              <p>{{ category.description }}</p>

              <button type="button" class="text-link text-button" @click="openGallery(category)">

                Echar un vistazo <span>↗</span>

              </button>

            </div>

          </article>

        </div>

        <div class="center-action">

          <a class="button button-dark" :href="generalMessage" target="_blank" rel="noopener noreferrer">

            Cotiza por WhatsApp

          </a>

        </div>

      </section>

      <section id="servicios" class="services-section section-padding">

        <div class="services-layout">

          <div class="services-copy">

            <p class="eyebrow">LO QUE HACEMOS</p>

            <h2>Servicios para renovar y cuidar tus espacios</h2>

            <p>

              Conoce los servicios que ofrecemos para la instalación, mantenimiento,

              limpieza y renovación de tus espacios.

            </p>

            <a class="button button-primary" :href="messageFor('información sobre servicios')" target="_blank" rel="noopener noreferrer">

              Consultar un servicio

            </a>

          </div>

          <div class="services-list">

            <ul>

              <li v-for="service in services" :key="service">

                <span class="service-check">✓</span>

                <span>{{ service }}</span>

              </li>

            </ul>

          </div>

        </div>

      </section>

      <section id="muestrarios" class="projects-section section-padding">

        <div class="section-heading">

          <p class="eyebrow">MUESTRARIOS</p>

          <h2>Conoce nuestros acabados</h2>

          <p>

            Explora algunas de las opciones de pisos y acabados disponibles para tus espacios.

          </p>

        </div>

        <div class="projects-grid">

          <article v-for="finish in finishes" :key="finish.name" class="project-card">

            <img :src="finish.image" :alt="finish.name" loading="lazy" />

            <div class="project-caption">

              <div>

                <h3>{{ finish.name }}</h3>

                <p>{{ finish.description }}</p>

              </div>

              <button type="button" @click="openGallery(finish)" :aria-label="`Ver muestrario de ${finish.name}`">↗</button>

            </div>

          </article>

        </div>

        <p class="gallery-note">

          Las imágenes son referencias ilustrativas; consulta disponibilidad de modelos y acabados por WhatsApp.

        </p>

      </section>

      <section class="quote-banner">

        <div>

          <p class="eyebrow">¿QUÉ NECESITAS PARA TU ESPACIO?</p>

          <h2>Cuéntanos qué espacio quieres transformar.</h2>

          <p>Contáctanos para recibir información sobre nuestros productos y servicios.</p>

        </div>

        <a class="button button-light" :href="generalMessage" target="_blank" rel="noopener noreferrer">

          Hablar por WhatsApp

        </a>

      </section>

      <section id="ubicacion" class="location-section section-padding">

        <div class="location-copy">

          <p class="eyebrow">VISÍTANOS</p>

          <h2>Estamos en Salamanca, Guanajuato</h2>

          <p>{{ address }}</p>

          <a class="text-link" :href="mapLink" target="_blank" rel="noopener noreferrer">

            Abrir ubicación en Google Maps <span>↗</span>

          </a>

        </div>

        <a class="map-container" :href="mapLink" target="_blank" rel="noopener noreferrer" aria-label="Ver ubicación en Google Maps">

          <iframe

            title="Mapa de Proyectos Modernos en Decoración en Salamanca, Guanajuato"

            :src="`https://maps.google.com/maps?q=${encodeURIComponent(address)}&output=embed`"

            loading="lazy"

            referrerpolicy="no-referrer-when-downgrade"

          ></iframe>

          <span class="map-label">Ver mapa ↗</span>

        </a>

      </section>

      <section id="contacto" class="contact-section section-padding">

        <div class="contact-heading">

          <p class="eyebrow">CONTACTO</p>

          <h2>Estamos para ayudarte</h2>

          <p>Solicita información o una cotización directamente con nosotros.</p>

        </div>

        <div class="contact-grid">

          <a class="contact-card contact-whatsapp" :href="generalMessage" target="_blank" rel="noopener noreferrer">

            <span class="contact-icon">✆</span>

            <h3>WhatsApp</h3>

            <p>+52 1 464 221 7051</p>

            <span class="contact-link">Escríbenos ↗</span>

          </a>

          <a class="contact-card" :href="mapLink" target="_blank" rel="noopener noreferrer">

            <span class="contact-icon">⌖</span>

            <h3>Visítanos</h3>

            <p>{{ address }}</p>

            <span class="contact-link">Cómo llegar ↗</span>

          </a>

          <div class="contact-card">

            <span class="contact-icon">◎</span>

            <h3>Redes sociales</h3>

            <p>Conoce más sobre nuestros productos y novedades.</p>

            <div class="social-links">

              <a

                v-for="social in socialLinks"

                :key="social.name"

                :href="social.url"

                :aria-label="social.label"

                target="_blank"

                rel="noopener noreferrer"

              >

                {{ social.name }}

              </a>

            </div>

          </div>

        </div>

      </section>

    </main>

    <footer class="footer">

      <a class="footer-brand" href="#inicio">

        <img class="footer-logo" src="/images/logop-negro-dorado.png" alt="" />

        <span>Proyectos Modernos en Decoración</span>

      </a>

      <p>Soluciones para crear espacios elegantes, confortables y modernos.</p>

      <div class="footer-socials">

        <a v-for="social in socialLinks" :key="social.name" :href="social.url" target="_blank" rel="noopener noreferrer">

          {{ social.name }}

        </a>

      </div>

      <small>© {{ new Date().getFullYear() }} Proyectos Modernos en Decoración. Todos los derechos reservados.</small>

    </footer>

    <div v-if="selectedGallery" class="gallery-modal" role="dialog" aria-modal="true" :aria-label="`Galería de ${selectedGallery.name}`">

      <button class="modal-backdrop" type="button" aria-label="Cerrar galería" @click="closeGallery"></button>

      <div class="gallery-panel">

        <div class="gallery-header">

          <div>

            <p class="eyebrow">MUESTRARIO</p>

            <h2>{{ selectedGallery.name }}</h2>

          </div>

          <button class="modal-close" type="button" aria-label="Cerrar galería" @click="closeGallery">×</button>

        </div>

        <div class="modal-gallery-grid">

          <article v-for="(image, index) in selectedGallery.gallery" :key="image" class="modal-gallery-item">

            <button

              class="image-open-button"

              type="button"

              :aria-label="`Abrir imagen ${index + 1} de ${selectedGallery.name}`"

              @click="openImage(image)"

            >

              <img :src="image" :alt="`${selectedGallery.name} ${index + 1}`" />

            </button>

            <a class="button button-primary" :href="messageFor(selectedGallery.name)" target="_blank" rel="noopener noreferrer">

              Solicitar información

            </a>

          </article>

        </div>

      </div>

    </div>

    <div v-if="selectedImage" class="image-viewer" role="dialog" aria-modal="true" aria-label="Imagen ampliada">

      <button class="image-viewer-backdrop" type="button" aria-label="Cerrar imagen" @click="closeImage"></button>

      <div class="image-viewer-panel">

        <button class="modal-close image-viewer-close" type="button" aria-label="Cerrar imagen" @click="closeImage">×</button>

        <img :src="selectedImage" alt="Imagen ampliada" />

      </div>

    </div>

    <a

      class="whatsapp-float"

      :href="generalMessage"

      target="_blank"

      rel="noopener noreferrer"

      aria-label="Contactar a Proyectos Modernos en Decoración por WhatsApp"

      title="Cotiza por WhatsApp"

    >

      <svg viewBox="0 0 32 32" aria-hidden="true">

        <path d="M16 3.2A12.6 12.6 0 0 0 5.1 22.1L3.5 28.7l6.8-1.8A12.6 12.6 0 1 0 16 3.2Zm0 22.9a10.2 10.2 0 0 1-5.2-1.4l-.4-.2-4 .9 1-3.9-.3-.4A10.2 10.2 0 1 1 16 26.1Zm5.6-7.7c-.3-.2-1.8-.9-2.1-1-.3-.1-.5-.2-.7.2-.2.3-.8 1-1 1.2-.2.2-.4.2-.7.1-.3-.2-1.3-.5-2.5-1.5-.9-.8-1.5-1.8-1.7-2.1-.2-.3 0-.5.1-.6l.5-.6c.2-.2.2-.3.3-.5.1-.2 0-.4 0-.6-.1-.2-.7-1.7-.9-2.3-.2-.6-.5-.5-.7-.5h-.6c-.2 0-.6.1-.9.4-.3.3-1.1 1.1-1.1 2.6s1.1 3 1.3 3.2c.2.2 2.2 3.4 5.3 4.7.7.3 1.3.5 1.7.6.7.2 1.4.2 1.9.1.6-.1 1.8-.7 2.1-1.4.3-.7.3-1.3.2-1.4-.1-.1-.3-.2-.6-.4Z"/>

      </svg>

    </a>

  </div>

</template>
