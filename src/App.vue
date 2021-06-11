<template>
  <div id="app">
    <h1 v-if="mensagem == ''">Digite algo para o papagaio falante repetir</h1>
    <div v-else>
      <h1  class="mensagem">Papagaio falante disse</h1>
      <h2>-{{mensagem}}</h2>
    </div>
    <img src="./assets/parrot.png" >
    <br>
    <input type="text" placeholder="digite aqui" v-model="mensagem"><br>
  </div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
      mensagem: "",
    }
  },
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  
}
h1{
  margin-top:50px;
   color:#8B3A3A;
}
h2{
  color: #CD5555;
}
input{
  width:200px;
  height:15px;
  margin-top:15px;
  background-color:#EEC591;
  border-color: #CD5555;
  border: 2.5px solid;
  color: #CD5555;
  text-color: red;
  text-align :center;
}

img{
  width:380px;
  height:240px
}
</style>
