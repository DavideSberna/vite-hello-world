<template>
  <nav>
    <AppTitle/>
  </nav>
  <header>
    <AppHero/>
  </header>
  <main>
    <AppMain/>
  </main>

   
</template>

<script>
import AppTitle from './components/AppTitle.vue';
import AppHero from './components/AppHero.vue';
import AppMain from './components/AppMain.vue';

export default{
  components: {
    AppTitle,
    AppHero,
    AppMain,
  }
}
</script>

<style lang="scss" scoped></style>