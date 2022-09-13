<script>
  export default {
    data: () => ({
      contador : 10,
    }),
    methods: {
      saludar(){
        console.ñog("Hola 10A | @");
      },
      incrementar(){
        this.contador++;
      },
      decrementar(){
        this.contador--;
      },
      resetear(){
        this.contador = 500;
      }
    }
  };
</script>

<template>
  <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125">
  <div class="container">
    <h1> Hola desde VUE.js 3</h1>
    <hr>
    <h2>Contandor {{ contador }}</h2>
      <button @click="incrementar()">+1</button>
      <button @click="decrementar()">-1</button>
      <button @click="resetear()">Reset</button>
  </div>
  <container>
    <div class="alert alert-primary" role="alert">
  Francisco Javier Tapia Rivera.
  <br>
  10A-DMI
</div>
  </container>
</template>

<style scoped>
  .container{
    text-align: center;
  }
  small{
    color: #666;
  }
  h1 {
    font-weight: bolder;
  }
  h2{
    font-size: 1.5rem;
  }
  button{
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 8px;
  }
</style>
