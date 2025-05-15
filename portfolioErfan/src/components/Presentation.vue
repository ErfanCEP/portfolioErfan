<template>
  <div class="fons d-flex align-items-center justify-content-center" style="min-height: 100vh;">
    <div class="row custom-width align-items-center justify-content-center">
      <!-- Texto centrado en la columna -->
      <div class="col-md-5 d-flex flex-column align-items-center justify-content-center">
        <div>
          <h1 class="erfan-ribas">Erfan Ribas</h1>
          <h2 class="text-center">Desarrollador Web</h2>
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
  background-color: rgb(153, 0, 255);
  height: 60vh;
  width: 100vw;
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
