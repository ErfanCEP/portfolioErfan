<template>
    <div class="container text-white  text-center">
        <div class="text-center m-5 p-5">
            <h1>ESTUDIOS</h1>
        </div>
        <div class="row m-5 align-items-center justify-content-center">
            <div class="col-6 my-5">
                <h1>DAW - Desarrollo de Aplicaciones Web</h1>
                <h4>Centre d'Estudis Politécnics</h4>
                <p>2023-2025</p>
            </div>
            <div class="col-6 my-5">
                <img :src=" '/img/CEP.png' " alt="Erfan Ribas" class="img-fluid rounded img-estudios" />
            </div>
             <div class="col-6 my-5">
                <h1>Grado Universitario Educación Infantil</h1>
                <h4>Blanquerna - Ramón Llull</h4>
                <p>2017-2022</p>
            </div>
            <div class="col-6 my-5">
                <img :src=" '/img/blq.jpg' " alt="Erfan Ribas" class="img-fluid rounded img-estudios" />
            </div>
             <div class="col-6 my-5">
                <h1>Bachillerato</h1>
                <h4>Institut Obert de Catalunya</h4>
                <p>2013-2015</p>
            </div>
            <div class="col-6 my-5">
                <img :src=" '/img/ioc.png' " alt="Erfan Ribas" class="img-fluid rounded img-estudios" />
            </div>
        </div>
    </div>
</template>



<style>
.img-estudios {
  max-width: 50%;
  height: auto;
}
</style>