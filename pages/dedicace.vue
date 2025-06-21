<script setup lang="ts">
// Récupérer l'élément image
const poupouImage = document.getElementById("poupouImage");

// Récupérer la fenêtre modale
const modal = document.getElementById("myModal");

// Récupérer le bouton de fermeture
const span = document.getElementsByClassName("close")[0];

// Ouvrir la modale quand l'image est cliquée
poupouImage.onclick = function() {
  modal.style.display = "block";
}

// Fermer la modale quand l'utilisateur clique sur le bouton de fermeture
span.onclick = function() {
  modal.style.display = "none";
}

// Fermer la modale si l'utilisateur clique en dehors de la fenêtre modale
window.onclick = function(event) {
  if (event.target === modal) {  // Utilisez === au lieu de ==
    modal.style.display = "none";
  }
}
</script>

<template>
  <h1>Neuilles de CESI</h1>
  <p>Timothée, tu sens les pieds</p>

  <!-- Image de poupou avec un ID -->

  <!-- La fenêtre modale -->
  <div id="myModal" class="modal">
    <div class="modal-content">
      <span class="close">&times;</span>
      <p id="modalText">Poupou est dans l'océan</p> <!-- Texte initial -->
    </div>
  </div>
</template>

<style scoped>
/* Style global de la page */
body {
  font-family: Arial, Helvetica, sans-serif;
  background-size: 90%;
  background-position: center center;
  background-attachment: fixed;
  margin: 0;
  height: 100vh;
  background-color: lightblue;
}
h1 {
  font-family: "Roboto Light", "Times New Roman", sans-serif;
  text-align: center;
  color: white;
  font-size: 3rem;
  margin-top: 40%;
}
p {
  color: hotpink;
  text-align: center;
  font-size: 2rem;
}

/* Style de la modale */
.modal {
  display: none;
  position: fixed;
  z-index: 1;
  left: 10%;
  top: 10%;
  width: 50%;
  height: 50%;
  background-color: hotpink;
  padding-top: 60px;
}
.modal-content {

background-color: lightblue;
margin: 5% auto;
padding: 20px;
border: 1px solid #888;
width: 50%;
text-align: center;
font-size: 1.5rem;
border-radius: 8px; /* Bords arrondis pour plus d'esthétique */
}
/* Style du bouton de fermeture */
.close {
  color: #aaa;
  font-size: 28px;
  font-weight: bold;
  position: absolute;
  top: 10px;
  right: 10px;
}
.close:hover,
.close:focus {
  color: black;
  text-decoration: none;
  cursor: pointer;
}

/* Effet au survol de l'image */
img {
  cursor: pointer;
  display: block;
  margin: 0 auto;
  transition: transform 0.2s ease-in-out;
}
img:hover {
  transform: scale(1.1); /* Effet de zoom au survol */
}
</style>