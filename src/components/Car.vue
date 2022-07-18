<template>
  <h2>Coche</h2>
  <p>Marca: {{ brand }}</p>
  <p>Color: {{ color[3] }}</p>
  {{mesage.text}}
</template>

<script>

export default {
   /*  data(){
        return{
            brand:"Audi",
            color:["azul", 'rojo','verde','amarillo'],
            mesage:{
                title:"hello world",
                text:"good bye"
            }


        }
    } */
    setup(){
        const brand="Audi";
        const color=["azul", 'rojo','verde','amarillo']
        const mesage={
            title:"esta es una prueba",
            text:"bienvenido"
        }
        return{
            brand,
            color,
            mesage
        }
    }
  
}
</script>

<style>

</style>