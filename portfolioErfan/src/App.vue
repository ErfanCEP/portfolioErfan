<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import Presentation from './components/Presentation.vue'
import Navbar from './components/Navbar.vue'
import Me from './components/Me.vue'
import Experiencia from './components/Experiencia.vue'
import Estudios from './components/Estudios.vue'
import Proyectos from './components/Proyectos.vue'
import Skills from './components/Skills.vue'
</script>


<template>
  <div>
    <header>
      <Navbar/>
    </header>
    <main class="">
      <section id="erfan">
        <Presentation/>
      </section>
      <section id="sobre-mi">
        <Me/>
      </section>
      <section id="proyectos">
        <Proyectos/>
      </section>
      <section id="experiencia">
        <Experiencia/>
      </section>
      <section id="estudios">
        <Estudios/>
      </section>
      <section id="skills">
        <Skills/>
      </section>
    </main>
  <footer>
  <div class="footer-overlay">
    <div class="footer-content text-center">
      <div class="footer-icons mb-2">
        <a href="https://github.com/" target="_blank" class="footer-icon mx-2" title="GitHub">
          <i class="bi bi-github"></i>
        </a>
        <a href="https://linkedin.com/" target="_blank" class="footer-icon mx-2" title="LinkedIn">
          <i class="bi bi-linkedin"></i>
        </a>
        <a href="mailto:erfan@email.com" class="footer-icon mx-2" title="Email">
          <i class="bi bi-envelope"></i>
        </a>
      </div>
      <p class="mb-0">© 2025 Erfan Ribas · Portfolio</p>
    </div>
  </div>
</footer>
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
<style>
main {
    background-image: url('/img/bg4-portfolio.avif');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: fixed;
    min-height: 100vh;
}

footer {
  position: relative;
  background-image: url('/img/footer.jfif');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  min-height: 200px; /* Aumenta la altura aquí */
  color: #fff;
  font-family: 'Montserrat', Arial, sans-serif;
  letter-spacing: 1px;
}

.footer-overlay {
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  background: rgba(30, 0, 60, 0.7); /* Morado oscuro semitransparente */
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}



@media (max-width: 600px) {
  .footer-content {
    font-size: 0.9rem;
  }
  .footer-icons {
    font-size: 1.5rem;
  }
}
</style>
