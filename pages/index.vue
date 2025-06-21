<script setup lang="ts">

</script>

<template>
  <div class="ocean">

    <div class="wrapper">
      <div class="text-white flex justify-center alt-font big">
        <span data-aos="fade-right" data-aos-duration="2000" data-aos-delay="600">T</span>
        <span data-aos="fade-right" data-aos-duration="2000" data-aos-delay="300">I</span>
        <span data-aos="fade" data-aos-duration="2000">D</span>
        <span data-aos="fade-left" data-aos-duration="2000" data-aos-delay="300">E</span>
        <span data-aos="fade-left" data-aos-duration="2000" data-aos-delay="600">S</span>
      </div>

      <div class="flex text-white justify-around alt-font">
        <a href="/contact" data-aos="fade" data-aos-duration="2000" data-aos-delay="600" class="text-4xl z-10 hover:scale-105 hover:drop-shadow-2xl hover:text-gray-300 transition-all">Contact</a>
        <a href="#video" data-aos="fade" data-aos-duration="2000" data-aos-delay="600" class="text-4xl z-10 hover:scale-105 hover:drop-shadow-2xl hover:text-gray-300 transition-all">Vidéo</a>
      </div>
    </div>

    <div class="flex justify-center pt-64">
      <img src="/img/humain.svg" data-aos="fade-up" data-aos-duration="3000" data-aos-delay="900" alt="Humain">
    </div>

    <div id="video" class="test">
    </div>
    <p>zqdzqd</p>
  </div>
</template>

<style scoped>
.alt-font {
  font-family: 'Sigmar', sans-serif;
}

.big {
  letter-spacing: 50px;
  font-size: 20vw;
  font-weight: 800;
}

.test {
  height: 4000px;
}

.wrapper {
  position:fixed;
  top: 0;
  left: 0;
  right: 0;
  width: 500px;
  margin: 0 auto;
}
</style>