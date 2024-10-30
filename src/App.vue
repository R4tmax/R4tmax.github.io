<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <h1 class="header-name">
      <RouterLink
        active-class="header-name-rl-override"
        exact-active-class="header-name-rl-override"
        to="/"
        >Martin Kadlec</RouterLink
      >
    </h1>
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
    <div class="footer-item">&copy; Martin Kadlec - 2024</div>
    <div class="footer-item">
      <div class="footer-subitem">
        Hosted via Github Pages
        <i class="fa-brands fa-github" aria-hidden="true"></i>
        - <a href="https://github.com/R4tmax/R4tmax.github.io" target="_blank">Repository</a>
      </div>
    </div>
    <div class="footer-item">
      <div class="footer-subitem">
        <a href="mailto:kadm09@vse.cz" target="_blank">
          <i class="fa-regular fa-envelope"></i> Napište mi!</a
        >
      </div>
      <div class="footer-subitem">
        <a href="https://github.com/R4tmax" target="_blank">
          <i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a
        >
      </div>
      <!-- <div class="footer-subitem">Spolupráce?</div> -->
    </div>
  </footer>
</template>
