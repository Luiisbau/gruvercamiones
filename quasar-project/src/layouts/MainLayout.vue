<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-white text-white" style="height: 3rem;">
      <q-toolbar>
        <q-toolbar-title class="custom-margin">
          <div class = "home">
          <img alt="Quasar logo" src="/icons/logo.png" />

          <a href="#home-section" class="texto-home no-underline">Home</a>

          <a href="#home-section" class="texto-home no-underline">Carga</a>

          <a href="#home-section" class="texto-home no-underline">Pasaje</a>

          <a href="#home-section" class="texto-home no-underline">Seminuevos</a>

          <a href="#home-section" class="texto-home no-underline">postventa</a>

          <a href="#home-section" class="texto-home no-underline">U</a>
        </div>
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <!-- Sección "Home" -->

      <div class="background-container">
      <div class="contenedor">
      <h1>ENMOVIMIENTO</h1>
    </div>
    </div>

    <div class="center-text">
  <h2>Gruver Camiones</h2>
  <p>Soluciones en Transporte</p>
  <div class="horizontal-line"></div>
</div>
<div class="text_inner"><p><span>En 1970, el Grupo incursiona en el &#8220;ramo camionero&#8221; quedando actualmente firmemente posicionado con la distribución de las marcas de camiones Mercedes Benz y Freightliner en las ciudades de Veracruz, Córdoba, Xalapa, Coatzacoalcos, Orizaba y Poza Rica, abarcando con esto el 100% del Estado de Veracruz y actualmente con una agencia en Jiutepec, Morelos, y Acapulco, Guerrero.</span></p>
<p>Formamos parte de GruVer, un Grupo dedicado principalmente al sector automotríz y camionero.</p>
<p>Las empresas que conforman Gruver están comprometidas con el servicio y la calidad, por ello, ofrecen las mejores marcas y productos en los mercados que operan, mismas que están respaldadas con una garantía por los fabricantes que las representan.</p>

<!--columnas de 3x3 -->
  <div class="word-columns">
    <div class="word-column">
      <p>Espíritu de servicio</p>
      <p>Respeto</p>
      <p>Compromiso</p>
    </div>
    <div class="word-column">
      <p>Honestidad</p>
      <p>Lealtad</p>
      <p>Integridad</p>
    </div>
    <div class="word-column">
      <p>Responsabilidad</p>
      <p>Confianza</p>
    </div>
  </div>
</div>

   <!-- imagenes -->
   <div class="additional-section">
    <div class="et_pb_blurb_content">
      <div class="et_pb_main_blurb_image">
        <!-- Imagen 1 -->
        <div class="image-container">
          <span class="et_pb_image_wrap et_pb_only_image_mode_wrap">
            <img class="additional-image" src="/icons/cascadia.jpg" alt="" />
          </span>
          <div class="additional-button">
            <q-btn color="primary" label="Carga" @click="handleButtonClick(1)" />
          </div>
        </div>

        <!-- Imagen 2 -->
        <div class="image-container">
          <span class="et_pb_image_wrap et_pb_only_image_mode_wrap">
            <img class="additional-image" src="/icons/M2-35K.jpg" alt="" />
          </span>
          <div class="additional-button">
            <q-btn color="primary" label="Carga" @click="handleButtonClick(2)" />
          </div>
        </div>

        <!-- Imagen 3 -->
        <div class="image-container">
          <span class="et_pb_image_wrap et_pb_only_image_mode_wrap">
            <img class="additional-image" src="/icons/OC-500-RF-2543.jpg" alt="" />
          </span>
          <div class="additional-button">
            <q-btn color="primary" label="Pasaje" @click="handleButtonClick(3)" />
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="q-pa-md">
    <q-carousel
      animated
      v-model="slide"
      arrows
      navigation
      infinite
    >
      <q-carousel-slide :name="1" img-src="https://cdn.quasar.dev/img/mountains.jpg" />
      <q-carousel-slide :name="2" img-src="https://cdn.quasar.dev/img/parallax1.jpg" />
      <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax2.jpg" />
      <q-carousel-slide :name="4" img-src="https://cdn.quasar.dev/img/quasar.jpg" />
    </q-carousel>
  </div>

  </q-layout>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref(1)
    }
  }
}
</script>
<style scoped>

</style>
