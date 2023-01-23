<script setup lang="ts">
import CreditsComponent from './components/CreditsComponent.vue';
import IntroComponent from './components/IntroComponent.vue'
import NavigationBar from './components/NavigationBar.vue'
import NewTextFile from './components/NewTextFile.vue';
import SearchComponent from './components/SearchComponent.vue';
</script>

<template>
  <NavigationBar/>
  <IntroComponent/>
  <SearchComponent/>
  <CreditsComponent/>
  <NewTextFile/>
</template>
