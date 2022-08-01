<template>
  <div id="app">
    <h1 v-if="mensagem == ''">Digite algo para o papagaio falante repetir</h1>
    <div v-else>
      <h1  class="mensagem">Papagaio falante disse</h1>
      <h2>{{mensagem}}</h2>
    </div>
    <img src="./assets/parrot.png" >
    <br>
    <input type="text" placeholder="Digite aqui" v-model="mensagem"><br>
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
  color:#8f3131;
}
h2{
  color: #CD5555;
}
input{
  width:500px;
  height:30px;
  margin-top:15px;
  background-color:#f2cdcb;
  border-color: #d77a7a;
  border: 2.5px solid;
  color: #f19292;
  font-size:15px;
  text-align :center;
}


img{
  width:480px;
  height:300px
}
</style>
