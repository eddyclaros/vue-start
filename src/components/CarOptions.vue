<template>
  <h2>Coche Options</h2>
  <p>Marca: {{ brand }}</p>
  <p>Modelo: {{ model }}</p>
  <p>Potencia: {{ power }} cv</p>

  <button @click="upPower()">Aumentar</button>
  <button @click="downPower()">Disminuir</button>
</template>

<script>

export default {
    data(){
      return{
        brand:"Toyota",
        model:"prius",
        power:50

      }
    },
    methods:{
      upPower(){
        //console.log("Subiendo Potencia" + this.power  )
        this.power=this.power+10
      },
      downPower(){
        //console.log("Bajando Potencia"  )
        this.power=this.power-10
      }
    }
    
  
}
</script>

<style>

</style>