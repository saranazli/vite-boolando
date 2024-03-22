<script>

  export default{
    data(){
      return{
        immagine: 'boolean-logo.png'
      }
    },

    methods:{
      getImagePath(image){
        return new URL(`../assets/scss/img/${image}`, import.meta.url).href;
      }
    }
  }

</script>

<template>

  <header class="center">

      <section class="conteiner header">
        
        <div class="options">
          <span>Donna</span>
          <span>Uomo</span>
          <span>Bambino</span>
        </div>

        <div class="logo cont">
          <img class="logo" :src="getImagePath(immagine)" alt="logo">
        </div>

        <div>
          logino
        </div>

      </section>

  </header>
  
</template>

<style lang="scss" scoped>

  @use '../assets/scss/main.scss' as *;

  header{
    height: 80px;
    background-color: $bg_color_header;
    .conteiner.header{
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-height: 100%;
      .options{
        padding-right: 10px;
      }
      .logo.cont{
        max-width: 40%;
        max-height: 70%;
        img.logo{
          width: 40%;
          height: 50%;
        }
      }
    }
  }

</style>