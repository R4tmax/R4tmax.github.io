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
        </nav>
      </div>
  </header>

  <main>
    <RouterView />
  </main>

</template>

