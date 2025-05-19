<template>
  <div class="fons d-flex align-items-center justify-content-center" style="min-height: 100vh; position: relative; overflow: hidden;">
    <video autoplay muted loop playsinline class="bg-video">
  <source src="/img/video-bg.mp4" type="video/mp4" />
</video>
    <div class="row custom-width align-items-center justify-content-center position-relative" style="z-index:2;">
      <!-- Texto centrado en la columna -->
      <div class="col-md-5 d-flex flex-column align-items-center justify-content-center">
        <div>
          <h1 class="erfan-ribas text-white">Erfan Ribas</h1>
          <h2 class="text-center text-white">Desarrollador Web</h2>
        </div>
      </div>
      <!-- Imagen -->
      <div class="col-md-5 d-flex align-items-center justify-content-center">
        <img :src=" '/img/erfanus.jpg' " alt="Erfan Ribas" class="img-fluid rounded" />
      </div>
    </div>
  </div>
</template>

<style>
.fons {
  position: relative;
  height: 60vh;
  width: 100vw;
  overflow: hidden;
}

/* .fons::after {
  content: "";
  position: absolute;
  left: 0; right: 0; bottom: 0;
  height: 120px;
  z-index: 2;
  pointer-events: none;
  background: linear-gradient(
    to bottom,
    rgba(0,0,0,0) 0%,
    #6200e210 100%
  );
} */


.bg-video {
  position: absolute;
  top: 0; left: 0; width: 100%; height: 100%;
  object-fit: cover;
  z-index: 1;
}

.fons > .row {
  position: relative;
  z-index: 2;
}

.erfan-ribas {
  font-size: 15rem;
}

/* Nueva clase para reducir el ancho del contenedor */
.custom-width {
  width: 80%; /* o prueba 70% o menos según lo que necesites */
  margin: 0 auto;
}
</style>
