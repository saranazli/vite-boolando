<script>

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
        <img class="logo" src="./img/boolean-logo.png" alt="logo">
      </div>

      <div>
        logino
      </div>

    </section>
  </header>
  
</template>

<style lang="scss">

  @use '../assets/scss/partials/_utilities';

  header{
    height: 80px;
    background-color: rgba(255,105,0,255);
      .conteiner.header{
        display: flex;
        align-items: center;
        justify-content: space-between;
        max-height: 100%;
        .options{
          padding-right: 10px;
        }
      }
  }

</style>