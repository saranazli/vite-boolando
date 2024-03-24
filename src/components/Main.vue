<script>
  import {myCards} from '../assets/data/db'
  import Card from '../components/partials/Card.vue'

  export default {
    components:{
      Card
    }
  }
</script>

<template>
  
  <main class="center">
    <div class="conteiner cards center">

      <Card />
      <Card />
      <Card />
      <Card />

    </div>
  </main>

</template>

<style lang="scss">

  @use '../assets/scss/main.scss';

  
  .conteiner.cards{
    flex-wrap: wrap;
    margin-top: 50px;
    margin-bottom: 50px;
  }


</style>