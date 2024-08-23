<template>
  <div class="bio-container">
    <div class="bio-header">
      <img src="/src/assets/fonts/images (1).jpeg" alt="John Doe" class="profile-picture" />
      <h1>John Doe</h1>
      <p class="job-title">Développeur Full-Stack & Architecte Logiciel</p>
      <p class="location">San Francisco, CA, USA</p>
    </div>
    <div class="bio-content">
      <section class="bio-section">
        <h2>À propos de John</h2>
        <p>
          John Doe est un développeur full-stack et architecte logiciel avec plus de 15 ans d'expérience dans la
          création de solutions technologiques innovantes. Il est passionné par le développement d'applications
          web performantes et évolutives, ainsi que par la conception de systèmes logiciels robustes.
        </p>
        <p>
          Expert en JavaScript, Python, et Java, John a travaillé pour des entreprises de premier plan dans la Silicon
          Valley, contribuant à la réussite de nombreux projets à grande échelle. Il est également un fervent défenseur
          des bonnes pratiques de développement, comme le TDD (Test Driven Development) et l'intégration continue.
        </p>
      </section>

      <section class="bio-section">
        <h2>Compétences Techniques</h2>
        <ul class="skills-list">
          <li>JavaScript (React, Vue.js, Node.js)</li>
          <li>Python (Django, Flask)</li>
          <li>Java (Spring Boot, Hibernate)</li>
          <li>Base de données (MySQL, PostgreSQL, MongoDB)</li>
          <li>DevOps (Docker, Kubernetes, CI/CD)</li>
          <li>Cloud (AWS, Google Cloud, Azure)</li>
        </ul>
      </section>

      <section class="bio-section">
        <h2>Expérience Professionnelle</h2>
        <div class="experience-item">
          <h3>Lead Developer & Architecte Logiciel</h3>
          <p class="experience-company">TechCorp Solutions, 2018 - Présent</p>
          <ul>
            <li>Conception et développement d'architectures microservices pour des applications cloud.</li>
            <li>Gestion d'une équipe de 10 développeurs, assurant la qualité du code et la livraison en temps voulu.</li>
            <li>Implémentation de pipelines CI/CD pour automatiser les déploiements.</li>
          </ul>
        </div>

        <div class="experience-item">
          <h3>Développeur Full-Stack Senior</h3>
          <p class="experience-company">Innovatech, 2013 - 2018</p>
          <ul>
            <li>Développement d'applications web complexes utilisant React et Node.js.</li>
            <li>Optimisation des performances des applications existantes, réduisant les temps de chargement de 30%.</li>
            <li>Collaboration avec les équipes de design pour créer des interfaces utilisateur intuitives.</li>
          </ul>
        </div>

        <div class="experience-item">
          <h3>Développeur Web</h3>
          <p class="experience-company">Webify, 2009 - 2013</p>
          <ul>
            <li>Création de sites web dynamiques et interactifs pour divers clients.</li>
            <li>Intégration d'API tierces pour étendre les fonctionnalités des applications.</li>
            <li>Maintenance et mise à jour régulière des sites existants pour garantir leur sécurité.</li>
          </ul>
        </div>
      </section>

      <section class="bio-section">
        <h2>Formation</h2>
        <div class="education-item">
          <h3>Master en Informatique</h3>
          <p class="education-school">Université de Stanford, 2007 - 2009</p>
        </div>
        <div class="education-item">
          <h3>Licence en Informatique</h3>
          <p class="education-school">Université de Californie, Berkeley, 2003 - 2007</p>
        </div>
      </section>

      <section class="bio-section">
        <h2>Projets Notables</h2>
        <div class="project-item">
          <h3>Application de Gestion de Projets "TaskMaster"</h3>
          <p>
            Un outil de gestion de projets en temps réel utilisé par plus de 100 000 utilisateurs dans le monde entier.
            John a dirigé l'équipe de développement pour créer une interface utilisateur réactive et une API backend robuste.
          </p>
        </div>
        <div class="project-item">
          <h3>Plateforme d'E-Commerce "ShopEase"</h3>
          <p>
            Développement d'une plateforme d'e-commerce complète avec gestion des stocks, traitement des paiements,
            et analyse des ventes. L'application a permis à de petites entreprises d'augmenter leurs ventes en ligne de 50%.
          </p>
        </div>
      </section>

      <section class="bio-section">
        <h2>Centres d'Intérêt</h2>
        <p>
          En dehors de son travail, John est un passionné de photographie et aime voyager à travers le monde pour capturer
          des moments uniques. Il est également un adepte de la course à pied et a participé à plusieurs marathons.
        </p>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Bio'
}
</script>

<style scoped>
.bio-container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  font-family: 'Roboto', Arial, sans-serif;
  color: #333;
  background-color: #f9f9f9;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
}

.bio-header {
  text-align: center;
  margin-bottom: 30px;
}

.profile-picture {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  margin-bottom: 15px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
}

.job-title {
  font-size: 1.4em;
  color: #007BFF;
  margin-bottom: 5px;
}

.location {
  font-size: 1em;
  color: #777;
}

.bio-content {
  margin-top: 20px;
}

.bio-section {
  margin-bottom: 30px;
}

.bio-section h2 {
  font-size: 1.8em;
  color: #007BFF;
  margin-bottom: 15px;
  border-bottom: 2px solid #007BFF;
  padding-bottom: 5px;
}

.bio-section p,
.bio-section ul {
  font-size: 1.1em;
  line-height: 1.8;
  color: #555;
}

.skills-list {
  list-style-type: none;
  padding: 0;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 10px;
}

.skills-list li {
  background-color: #e7f3ff;
  padding: 10px;
  border-radius: 4px;
  text-align: center;
  color: #007BFF;
}

.experience-item,
.education-item,
.project-item {
  margin-bottom: 20px;
}

.experience-item h3,
.education-item h3,
.project-item h3 {
  font-size: 1.4em;
  color: #333;
  margin-bottom: 5px;
}

.experience-company,
.education-school {
  font-size: 1.1em;
  color: #777;
  margin-bottom: 10px;
}

.project-item p {
  margin-bottom: 10px;
  color: #555;
}

@media (max-width: 600px) {
  .skills-list {
    grid-template-columns: 1fr;
  }
}
</style>
