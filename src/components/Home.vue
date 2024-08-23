<template>
  <div class="home-container">
    <!-- Section de bienvenue avec image de fond -->
    <div class="hero-section">
      <div class="overlay">
        <h1 class="hero-title">Bienvenue dans l'univers de John Doe</h1>
        <p class="hero-subtitle">Développeur aguerri, passionné par la technologie et l'innovation</p>
        <button class="cta-button" @click="goToProjects">Découvrir les projets</button>
        <button class="cta-button" @click="goToContact">Contactez-moi</button>
      </div>
    </div>

    <!-- Section de présentation rapide -->
    <section class="about-section">
      <h2 class="section-title">Qui est John Doe?</h2>
      <p class="about-description">
        Avec plus de 10 ans d'expérience dans le développement web, John Doe a travaillé sur des projets innovants et complexes pour des entreprises de premier plan. 
        Spécialisé en développement frontend et backend, il aime créer des solutions efficaces qui allient performance et design.
      </p>
      <div class="about-stats">
        <div class="stat-item">
          <h3>100+</h3>
          <p>Projets terminés</p>
        </div>
        <div class="stat-item">
          <h3>50K+</h3>
          <p>Lignes de code</p>
        </div>
        <div class="stat-item">
          <h3>10+</h3>
          <p>Années d'expérience</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Home',
  methods: {
    goToProjects() {
      this.$router.push('/projects');
    },
    goToContact() {
      this.$router.push('/contact');
    },
  },
};
</script>

<style scoped>
/* Conteneur principal */
.home-container {
  font-family: 'Roboto', Arial, sans-serif;
  color: #333;
  background-image: url("src/assets/fonts/images (8).jpeg");
}

/* Section de bienvenue avec image de fond */
.hero-section {
  background-image: url('https://via.placeholder.com/1200x600?text=Welcome+to+John+Doe%27s+World');
  background-size: cover;
  background-position: center;
  height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.overlay {
  background-color: rgba(0, 0, 0, 0.6);
  color: #fff;
  text-align: center;
  padding: 40px;
  border-radius: 8px;
}

.hero-title {
  font-size: 3em;
  margin-bottom: 20px;
}

.hero-subtitle {
  font-size: 1.5em;
  margin-bottom: 30px;
}

.cta-button {
  background-color: #007BFF;
  color: #fff;
  border: none;
  padding: 15px 30px;
  font-size: 1.2em;
  border-radius: 5px;
  cursor: pointer;
  margin: 10px;
  transition: background-color 0.3s ease;
}

.cta-button:hover {
  background-color: #0056b3;
}

/* Section de présentation rapide */
.about-section {
  padding: 60px 20px;
  background-color: #f9f9f9;
  text-align: center;
}

.section-title {
  font-size: 2.5em;
  color: #007BFF;
  margin-bottom: 40px;
}

.about-description {
  font-size: 1.2em;
  color: #555;
  margin-bottom: 40px;
}

.about-stats {
  display: flex;
  justify-content: center;
  gap: 50px;
}

.stat-item {
  text-align: center;
}

.stat-item h3 {
  font-size: 2.5em;
  color: #007BFF;
}

.stat-item p {
  font-size: 1.1em;
  color: #555;
}
</style>
