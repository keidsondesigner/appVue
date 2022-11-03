<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <DefaultButton text="Olá mundo" />
  <DefaultInputVue
    text="Data de Nascimento"
    message="Valor incorreto, por favor digite novamente!"
  />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import DefaultButton from './components/DefaultButton.vue'
import DefaultInputVue from './components/DefaultInput.vue';


export default {
  name: 'App',
  components: {
    HelloWorld,
    DefaultButton,
    DefaultInputVue,
  }
}
</script>

<style>
* {
  padding:0;
  margin:0;
  vertical-align:baseline;
  list-style:none;
  border:0
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
