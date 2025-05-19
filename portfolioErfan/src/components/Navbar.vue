<template>
  <nav class="navbar navbar-expand-lg navbar-dark fixed-top">
    <div class="container-fluid">
      <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item" v-for="id in sections" :key="id">
            <a
              class="nav-link"
              :class="{ active: activeSection === id }"
              :href="'#' + id"
            >
              {{ id === 'erfan' ? 'Erfan' :
                 id === 'sobre-mi' ? 'Sobre mí' :
                 id.charAt(0).toUpperCase() + id.slice(1) }}
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const activeSection = ref('erfan')

const sections = [
  'erfan',
  'sobre-mi',
  'proyectos',
  'experiencia',
  'estudios',
  'skills'
]

function onScroll() {
  for (const id of sections) {
    const el = document.getElementById(id)
    if (el) {
      const rect = el.getBoundingClientRect()
      if (rect.top <= 80 && rect.bottom > 80) {
        activeSection.value = id
        break
      }
    }
  }
}

onMounted(() => {
  window.addEventListener('scroll', onScroll)
  onScroll()
})

onUnmounted(() => {
  window.removeEventListener('scroll', onScroll)
})
</script>

<style scoped>
.nav-link {
  position: relative;
  transition: color 0.2s;
}

.nav-link::after {
  content: "";
  display: block;
  width: 0;
  height: 2px;
  background: #fff;
  transition: width 0.3s;
  position: absolute;
  left: 0;
  bottom: 0;
}

.nav-link:hover::after,
.nav-link.active::after {
  width: 100%;
}

nav {
  background-color: #0f1623cc;


}
</style>