<script setup lang="ts">

</script>

<template>
  <div>
    <header>
      <h1>Bienvenue sur ma page avec une UI incroyable</h1>
      <button class="inutiles">Cliquez ici pour rien</button>
      <select class="menu-deroulant">
        <option value="option1">Option 1</option>
        <option value="option2">Option 2</option>
        <option value="option3">Option 3</option>
        <option value="option4">Option 4</option>
        <option value="option5">Option 5</option>
      </select>
    </header>

    <section>
      <h2>Regardé ma vidhéo de qalité</h2>
      <video width="1000" height="600" autoplay loop muted>
        <source src="ModX.mp4" type="video/mp4">
        <source src="brokenvideo.avi" type="video/avi">
        Votre navigateur ne supporte pas la balise vidéo.
      </video>
      <button class="inutiles">Cliquez pour changer de taille</button>
      <button class="inutiles">Cliquez ici aussi</button>
      <select class="menu-deroulant">
        <option value="option1">Option 1</option>
        <option value="option2">Option 2</option>
        <option value="option3">Option 3</option>
        <option value="option4">Option 4</option>
        <option value="option5">Option 5</option>
      </select>
    </section>

    <footer>
      <p>Créé avec amour par Moi <br> créé à partir du site https://modx-catamarans.com/modx-70/ </p>
      <button class="inutiles">Ne cliquez pas ici !</button>
    </footer>

    <select class="menu-deroulant">
      <option value="option1">Option 1</option>
      <option value="option2">Option 2</option>
      <option value="option3">Option 3</option>
      <option value="option4">Option 4</option>
      <option value="option5">Option 5</option>
    </select>
    <select class="menu-deroulant">
      <option value="option1">Option 1</option>
      <option value="option2">Option 2</option>
      <option value="option3">Option 3</option>
      <option value="option4">Option 4</option>
      <option value="option5">Option 5</option>
    </select>

    <div class="vague">
      <img src="vague.webp" alt="Vague défilante">
    </div>

    <div class="texte-tournant">
      <p>MODX 70 le bateau du futur</p>
      <p>Appliquer des technologies éprouvées de construction de bateaux de course et de performances de navigation à un voilier de plaisance hauturière.</p>
      <p>Le MODX 70 a été conçu et fabriqué dans un souci d’esthétique, de performance, de durabilité et d’autonomie. Une nouvelle génération de bateau offrant un mixte aile-moteur électrique, sans bruit, conciliant le plaisir d’un yachting assisté et le confort de vie du motor yacht. La construction composite légère est le fruit d’un travail approfondi avec le cabinet VPLP et d’un process de construction élaboré et pragmatique (40% bio-sourcés, 15% carbone,…).</p>
      <p>Le MODX 70 est avant tout un bateau hauturier permettant d’affronter des conditions difficiles tout en conservant un immense plaisir de navigation.</p>
      <p>Architectes navals : VPLP Design</p>
      <p>Design intérieur : Océan Développement / Pierre Frutschi Design</p>
      <p>Certification CE : A/B/C/D (en cours)</p>
      <p>Nombre de couchages : 8/10 passagers + 2/3 équipages</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MonComponent',
  // Ici, tu peux ajouter des données ou des méthodes si nécessaire
}
</script>

<style scoped>
/* Styles de la pire expérience utilisateur */

/* Corps de la page */
body {
  background-color: #ff00ff; /* Violet fluo */
  font-family: 'Comic Sans MS', cursive, sans-serif;
  color: #ffff00; /* Jaune vif */
  text-align: center;
  margin: 0;
  padding: 0;
}

/* Entête */
header {
  background-color: #ff0000; /* Rouge */
  color: #0000ff; /* Bleu */
  font-size: 50px;
  padding: 20px;
  text-transform: uppercase;
  border: 10px solid black;
}

/* Section vidéo */
section {
  background-color: #00ff00; /* Vert fluo */
  padding: 30px;
  margin: 50px;
  border: 10px dotted black;
  box-shadow: 0 0 30px rgba(0, 0, 0, 0.5);
}

/* Élément vidéo */
video {
  position: absolute;
  top: 100px;
  left: 200px;
  width: 1000px;  /* Vidéo démesurément grande */
  height: 600px;  /* Taille exagérée */
  transform: rotate(45deg);  /* Angle déformé */
  object-fit: cover;
  filter: grayscale(100%) brightness(200%) contrast(150%);
}

/* Boutons inutiles */
button {
  position: absolute;
  background-color: #ff0000; /* Rouge */
  color: #ffffff;
  border: 5px solid black;
  font-size: 20px;
  padding: 10px 20px;
  text-transform: uppercase;
  cursor: pointer;
  z-index: 10;
}

button:hover {
  background-color: #00ff00; /* Vert fluo au survol */
  color: #0000ff; /* Bleu */
}

/* Placement aléatoire des boutons inutiles */
button.inutiles:nth-child(odd) {
  top: 50px;
  left: 300px;
}

button.inutiles:nth-child(even) {
  top: 200px;
  left: 500px;
}

button.inutiles:nth-child(3) {
  top: 400px;
  left: 700px;
}

button.inutiles:nth-child(4) {
  top: 600px;
  left: 100px;
}

/* Menus déroulants qui prennent beaucoup de place */
select.menu-deroulant {
  font-size: 30px;
  padding: 15px;
  width: 400px; /* Largeur excessive pour les menus déroulants */
  height: 50px;
  background-color: #ff00ff;
  color: #ffff00;
  border: 5px solid #0000ff;
  margin: 20px 0;
}

select.menu-deroulant option {
  background-color: #ff0000;
  color: #0000ff;
  font-size: 20px;
}

/* Placement aléatoire des menus déroulants */
select.menu-deroulant:nth-child(odd) {
  position: absolute;
  top: 80px;
  left: 350px;
}

select.menu-deroulant:nth-child(even) {
  position: absolute;
  top: 250px;
  left: 600px;
}

footer {
  background-color: #ffff00; /* Jaune */
  color: #ff00ff; /* Rose */
  font-size: 30px;
  padding: 10px;
  position: fixed;
  bottom: 0;
  width: 100%;
  text-align: center;
  font-family: 'Comic Sans MS', sans-serif;
}

/* Image PNG de vague défilante */
.vague {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100px; /* Hauteur de l'image */
  overflow: hidden;
  z-index: 1;
}

.vague img {
  width: auto;
  height: 100%;
  animation: defilement 10s linear infinite; /* Animation pour faire défiler */
}

@keyframes defilement {
  0% {
    transform: translateX(100%); /* Démarre à droite */
  }
  100% {
    transform: translateX(-100%); /* Fini à gauche */
  }
}

/* Texte tournant lentement dans le coin bas à gauche */
.texte-tournant {
  position: absolute;
  bottom: 0;
  left: 0;
  font-size: 16px;
  color: #ffffff;
  text-align: left;
  width: 100%;
  animation: rotation 120s linear infinite; /* Rotation encore plus lente */
  padding: 10px;
}

@keyframes rotation {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
</style>
