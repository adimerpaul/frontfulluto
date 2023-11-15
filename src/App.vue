<template>
  <div>
    <h3>Suma de 2 numeros</h3>
    <input
    v-model="num1"
    type="number"/>
    <input
    v-model="num2"
    type="number"/>
    <br>
    <button @click="sumar">sumar</button>
    <br>
    <p>resultado {{ res }}</p>
    <Hola></Hola>
  </div>
</template>

<script>
import Hola from "@/components/Hola.vue"
export default {
  name: 'App',
  components:{
    Hola
  },
  data(){
    return{
      num1: 45,
      num2: 30,
      res: 0
    }
  },
  methods :{
    sumar(){
      this.res= this.num1+this.num2
    }
  }
}
</script>
<style>
html{
  background: gray;
}
</style>