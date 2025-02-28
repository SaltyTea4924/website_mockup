<script setup>
import HelloWorld from './components/HelloWorld.vue'
var guitar_images = ["guitar_1.jpg","guitar_2.jpg","guitar_3.jpg","guitar_4.jpg"]
var pedal_images = ["pedal_1.jpg", "pedal_2.jpg","pedal_3.jpg","pedal_4.jpg"]
</script>

<template>
  <header>

    <div>
      <HelloWorld msg="Gallery of guitars"/>
    <div v-for = "guitar in guitar_images">
            <img v-bind:src="guitar" height="200" width="125">
    </div>
    <HelloWorld msg ="Gallery of Pedals"/>
    <div v-for = "pedal in pedal_images">
      
      <img v-bind:src="pedal" height="200" width="125"></div>
    </div>
  </header>

  
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>