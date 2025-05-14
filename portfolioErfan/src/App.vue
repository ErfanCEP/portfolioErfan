<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import Presentation from './components/Presentation.vue'
import Navbar from './components/Navbar.vue'
import Me from './components/Me.vue'
import Experiencia from './components/Experiencia.vue'
import Estudios from './components/Estudios.vue'
// import Proyectos from './components/Proyectos.vue'
// import Skills from './components/Skills.vue'
</script>

<template>
  <div>
    <header>
      <Navbar />
    </header>
    <main>
      <Presentation/>
      <Me/>
      <Experiencia/>
      <Estudios/>
    </main>
    </div>
  

</template>

<!-- <style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style> -->
