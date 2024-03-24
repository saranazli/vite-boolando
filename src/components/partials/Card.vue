
<script>
  import { myCards } from '../../assets/data/db';

  export default{
    data(){
      return{
        myCards
      }
    }
  }


</script>


<template>

  <section class="conteiner-card">
    <img :src="myCards.products.frontImage" alt="">
  </section>
  

</template>


<style lang="scss" scoped>

@use '../../assets/scss/main.scss';

.conteiner-card{
  width: 400px;
  height: 700px;
  margin: 10px;
  position: relative;
}

</style>