

<template>
    <div class="painel">
    <h2 class="painel-titulo">{{titulo}}</h2>
    <slot class="painel-conteudo">
    </slot>
    </div>
</template>

<script>
    export default {
        props: ['titulo']
    }
</script>

<style scoped>
 .painel {
    padding: 0 auto;
    display: inline-block;
    margin: 5px;
    box-shadow: 0px 0px 5px 0px #888888;
    width: 200px;
    height: 100%;
    vertical-align: top;
    text-align: center;
  }

  .painel .painel-titulo {
    text-align: center;
    border: solid 2px;
    background: lightblue;
    margin: 0 0 15px 0;
    padding: 10px;
    text-transform: uppercase;
  }

  /* colocando todos os elementos do painel com box shadow */

  * {
    border-radius: 10px;
    border: none;
  }


</style>
