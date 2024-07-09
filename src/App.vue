<script>
import AppHeader from './components/AppHeader.vue'
import CharactersList from './components/CharactersList.vue'

export default { 
  name: "App",
  components:{
    AppHeader,
    CharactersList,
  }
}
</script>

<template>
  <AppHeader message="Yu-Gi-Oh Api"/>
  <main>
    <CharactersList />
  </main>
 
</template>

<style lang="scss">
@use './style/general.scss';


</style>
