<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>

  <header>
    <h1>Martin Kadlec</h1>
      <div class="nav-wrapper">
        <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
          <RouterLink to="/blog">Blog</RouterLink>
          <!-- <RouterLink to="/cv">CV</RouterLink> -->
        </nav>
      </div>
  </header>

  <main>
    <RouterView />
  </main>

  <footer>
    <div class="footer-item"> &copy; Martin Kadlec - 2024 </div>
    <div class="footer-item"> Hosted via Github Pages</div>
    <div class="footer-item"> 
      <div class="footer-subitem"><a href="mailto:kadm09@vse.cz" target="_blank" class="cv-quick-link">Napište mi!</a></div>
      <div class="footer-subitem"><a class="cv-card" href="https://github.com/R4tmax" target="_blank"> <i class="fa-brands fa-github" aria-hidden="true"></i>
        GitHub</a></div>
      <div class="footer-subitem">Spolupráce?</div>
    </div>
  </footer>
</template>

