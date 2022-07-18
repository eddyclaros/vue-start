<template>
  <h2>Coche Composition API</h2>
  <p>Marca: {{ brand }}</p>
  <p>Potencia: {{ power }}</p>
  <button @click="upPower">aumentar</button>
  <button @click="downPower">disminuir</button>
  
    <!-- <span v-for="(color,index) in colors" :key="index">{{index}}:{{color}}-</span> -->
   <!--  <ul>
        <li v-for="(color,index) in colors" :key="index">{{index}}:{{color}}</li>
    </ul>
  </p>
  <p>Potencias menores a 150</p>
  <ul>
    <template v-for="(p,index) in power" :key="index">
        <li v-if="p<150">{{p}}</li>
    </template>

  </ul>

  <p>Potencias mayores a 150</p>
  <ul>
    <template v-for="(p,index) in power" :key="index">
        <li v-if="p>=150">{{p}}</li>
    </template>

  </ul>


  {{mesage.text}} -->
</template>

<script>
import { ref } from "vue"
export default {
    setup(){
        const brand="Audi";
        let power=ref(40);
       /*  const colors=["azul", 'rojo','verde','amarillo']
        const mesage={
            title:"esta es una prueba",
            text:"bienvenido"
            
        }
        const power=[60,80,100,120,200,250,300,400,500]
        */

       const upPower=()=>{
        //console.log(power)
        power.value=power.value+1
       }
       const downPower=()=>{
        //console.log("disminuir potencia")
        power.value=power.value-1
       }
        return{
            brand,
            power,
            upPower,
            downPower
            /*colors,
            mesage,
            power
            */
        } 
    },
    
  
}
</script>

<style>

</style>