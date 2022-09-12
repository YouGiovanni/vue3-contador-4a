<script>
  export default{
    data: () =>({
      contador: 500,
    }),
    methods: {
      saludar(){
        console.log("Hola 4A");
      },
      incrementar(){
        this.contador ++;
      },
      decrementar(){
        this.contador --;
      },
      resetear(){
        this.contador=500;
      },
    }
  };
</script>

<template>
  <!-- CSS only -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx" crossorigin="anonymous">
  <div class="container">
    <img src="./assets/logo.svg" alt="Logo Vue" width="125" height="125">

    <small>
      <h1>Hola desde Vue.js</h1>
    </small>

    <hr>
    <br>

    <h2>Contador {{contador}}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="decrementar()">-1</button>
    <button @click="resetear()">Reset</button>

  </div>

  <br>
  <div class="nombre">
    <div class="alert alert-secondary" role="alert">
      You Giovanni Valencia Vazquez 4 "A"
    </div>

  </div>

</template>

<style scoped>
.container {
  text-align: center;
  background-color: #ddd;
}

h1 {
  font-weight: bolder;
  font-family: 'Oswald', sans-serif;
  color: gray;
}

small{
  color: grey;
}

.nombre {
  width: 200px;
  position: fixed;
  margin: 0px 900px;
  text-align: center;
}

h2{
  font-size: 2.5rem;
}

button{
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 8px;
}

</style>