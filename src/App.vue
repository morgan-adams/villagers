<template>
  <div id="app">
    <VillagerCard name="Marshal"
                  img="https://nookipedia.com/w/images/b/bb/Marshal_NL.png"
                  species="squirrel"/>
    <VillagerCard name="Lolly"
                  img="https://nookipedia.com/w/images/0/05/Lolly_NLa.png"
                  species="cat"/>
    <VillagerCard name="Rosie"
                  img="https://nookipedia.com/w/images/a/a1/Rosie_NLa.png"
                  species="cat"/>
    <VillagerCard name="Stitches"
                  img="https://nookipedia.com/w/images/b/b1/Stitches_NLa.png"
                  species="bear"/>
    <VillagerCard name="Diana"
                  img="https://nookipedia.com/w/images/c/c2/Diana_NLa.png"
                  species="deer"/>
    <VillagerCard name="Lucky"
                  img="https://nookipedia.com/w/images/2/25/Lucky_NLa.png"
                  species="dog"/>
  </div>
</template>

<script>
import VillagerCard from './components/VillagerCard.vue'

export default {
  name: 'app',
  components: {
    VillagerCard
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
