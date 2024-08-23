<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<template>
    <div class="navbar">
      <a href="/" class="icon">Focus</a>
      <nav>
        <ul>
          <li><a href="/about">Bio</a></li>
          <li><a href="/contact">Contact</a></li>
          <li><a href="/projects">Projets</a></li>
          <li><a href="/skills">Skills</a></li>
        </ul>
      </nav>
    </div>
    <RouterView />
</template>

<style scoped>
.navbar {
  border-bottom: 2px solid black;
  border-radius: 10px;
}
.icon {
  font-size: 20pt;
  font-weight: bold;
  color: blue;
  text-decoration: none;
}
ul {
  list-style: none;
  display: flex;
  gap: 15px;
  margin-right: 2rem;
}

</style>