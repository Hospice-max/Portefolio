<template>
  <section id="skills">
    <h2>Skills</h2>
    <ul>
      <li v-for="skill in skills" :key="skill.name">
        {{ skill.name }}: <progress :value="skill.level" max="100"></progress>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        { name: 'HTML', level: 90 },
        { name: 'CSS', level: 80 },
        { name: 'JavaScript', level: 85 },
        // Ajoutez d'autres compétences
      ]
    }
  }
}
</script>

<style scoped>

</style>