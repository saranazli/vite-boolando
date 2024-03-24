
<script>
  import { myCards } from '../../assets/data/db';

  export default{
    data(){
      return{
        myCards
      }
    },
    methods:{
      getImagePath(image){
        return new URL(`../../../public/img/${image}`, import.meta.url).href;
      }
    },
    computed:{
      cardCicle() {
        return (this.myCards.products);
      }
    }


  }


</script>


<template>

  <section 
  v-for="(item, index) in cardCicle" 
  :key="index" 
  class="conteiner-card">

    <div class="card-relaxed">

      <img :src="getImagePath(item.frontImage)" alt="img">

    </div>

    <div class="text relaxed">
      <span class="brand"> {{ item.brand }} </span>
      <h1 class="clothes-name"> {{ item.name }}</h1>
      <span class="solded-price"> {{ item.price }}</span>
    </div>

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