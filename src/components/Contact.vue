<template>
        <div class="contact-container">
            <h1 class="title">Contactez John Doe</h1>
        
            <div class="contact-info">
                <p><strong>Email:</strong> john.doe@example.com</p>
                <p><strong>Téléphone:</strong> +1 234 567 890</p>
                <p><strong>Adresse:</strong> 1234 Main Street, San Francisco, CA, USA</p>
            </div>
        
            <form class="contact-form" @submit.prevent="submitForm">
                <div class="form-group">
                    <label for="name">Nom</label>
                    <input type="text" id="name" v-model="form.name" required />
                </div>
        
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" v-model="form.email" required />
                </div>
        
                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea id="message" v-model="form.message" required></textarea>
                </div>
        
                <button type="submit" class="submit-button">Envoyer</button>
            </form>
        </div>
</template>

<script lang="ts">
export default {
    
  name: 'Contact',
  data() {
    return {
      form: {
        name: '',
        email: '',
        message: '',
      },
    };
  },
  methods: {
    submitForm() {
      // Exemple de traitement du formulaire
      console.log('Formulaire soumis:', this.form);
      alert(`Merci, ${this.form.name}. Votre message a été envoyé.`);
      this.resetForm();
    },
    resetForm() {
      this.form.name = '';
      this.form.email = '';
      this.form.message = '';
    },
  },
};
</script>

<style scoped>

.contact-container {
    max-width: 600px;
    margin: 0 auto;
    margin-top: 8rem;
    padding: 20px;
    font-family: 'Roboto', Arial, sans-serif;
    color: #333;
    background-color: #f9f9f9;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
}

.title {
    text-align: center;
    font-size: 2em;
    margin-bottom: 30px;
    color: #007BFF;
}

.contact-info {
    text-align: center;
    margin-bottom: 30px;
    font-size: 1.1em;
    color: #555;
}

.contact-form {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.form-group {
    display: flex;
    flex-direction: column;
}

.form-group label {
    font-size: 1.1em;
    margin-bottom: 5px;
    color: #007BFF;
}

.form-group input,
.form-group textarea {
    padding: 10px;
    font-size: 1em;
    border-radius: 5px;
    border: 1px solid #ccc;
}

.form-group textarea {
    resize: vertical;
    min-height: 100px;
}

.submit-button {
    padding: 10px 20px;
    font-size: 1.1em;
    color: #fff;
    background-color: #007BFF;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.submit-button:hover {
    background-color: #0056b3;
}
</style>
