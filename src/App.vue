<script setup>
import HelloWorld from './components/HelloWorld.vue'
import AppButton from './components/AppButton.vue';
// Methods
function addNews() {
  console.log('working!')
}
</script>

<template>
  <header>
    <div class="header">
       <img alt="Avantio logo" class="logo" src="./assets/Avantio-logo.svg" width="125" height="125" />

    <div class="wrapper">
      <AppButton text="Agregar nueva noticia" @click="addNews"></AppButton>
    </div>
    </div>
   
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
.header {
  width: 100%;
  display: flex;
  place-items: center;
  justify-content: space-around;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    /* place-items: center; */
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    /* display: flex; */
    /* place-items: flex-start; */
    flex-wrap: wrap;
  }
}
</style>
