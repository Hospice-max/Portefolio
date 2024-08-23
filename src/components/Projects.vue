<template>
  <div class="projects-container">
    <h1 class="title">Projets de John Doe</h1>
    <div class="projects-grid">
      <div class="project-card" v-for="project in projects" :key="project.id">
        <img :src="project.image" :alt="project.title" class="project-image" />
        <h2 class="project-title">{{ project.title }}</h2>
        <p class="project-description">{{ project.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Projects',
  data() {
    return {
      projects: [
        {
          id: 1,
          title: 'Application de Gestion de Projets "TaskMaster"',
          description:
            'Un outil de gestion de projets en temps réel utilisé par plus de 100 000 utilisateurs dans le monde entier. John a dirigé l\'équipe de développement pour créer une interface utilisateur réactive et une API backend robuste.',
          image: 'src/assets/Image/gestion.png',
        },
        {
          id: 2,
          title: 'Plateforme d\'E-Commerce "ShopEase"',
          description:
            'Développement d\'une plateforme d\'e-commerce complète avec gestion des stocks, traitement des paiements, et analyse des ventes. L\'application a permis à de petites entreprises d\'augmenter leurs ventes en ligne de 50%.',
          image: 'src/assets/Image/mockup.jpg',
        },
        {
          id: 3,
          title: 'Réseau Social "Connectify"',
          description:
            'Création d\'un réseau social innovant qui connecte les utilisateurs avec des intérêts communs. John a conçu l\'architecture backend et supervisé l\'intégration des fonctionnalités sociales.',
          image: 'src/assets/Image/maquette.jpg',
        },
        {
          id: 4,
          title: 'Application Mobile "FitTrack"',
          description:
            'Une application mobile de suivi de la condition physique qui permet aux utilisateurs de suivre leurs entraînements, leur nutrition et leurs progrès au fil du temps. John a développé l\'application avec une interface utilisateur intuitive et des fonctionnalités de synchronisation en temps réel.',
          image: 'src/assets/Image/ted.jpg',
        },
      ],
    };
  },
};
</script>

<style scoped>
.projects-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  font-family: 'Roboto', Arial, sans-serif;
  color: #333;
}

.title {
  text-align: center;
  font-size: 2.5em;
  margin-bottom: 40px;
  color: #007BFF;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
}

.project-card {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  padding: 20px;
  text-align: center;
}

.project-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 8px 8px 0 0;
}

.project-title {
  font-size: 1.5em;
  margin: 15px 0;
  color: #007BFF;
}

.project-description {
  font-size: 1.1em;
  color: #555;
  line-height: 1.6;
}
</style>
