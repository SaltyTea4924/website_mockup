<template>
  <div>
    <div>Onion {{ sum_onion }}</div>
    <button @click="sum_onion++">+</button><button @click="minusClick_Onion">-</button>
    <div>Tomatoes {{ sum_tomato }}</div>
    <button @click="sum_tomato++">+</button><button @click="minusClick_Tomato">-</button>
    <div>Chicken {{ sum_Chicken }}</div>
    <button @click="sum_Chicken++">+</button><button @click="minusClick_Chicken">-</button>
  </div>
</template>

<script>
  export default{
      data(){
        return{
          sum_onion: '0',
          sum_tomato: '0',
          sum_Chicken: '0'
        }
      },
      methods:{
        minusClick_Onion(){
          if (this.sum_onion > 0){
            this.sum_onion--;
          }},
          minusClick_Tomato(){
          if (this.sum_tomato > 0){
            this.sum_tomato--;
          }
        }, minusClick_Chicken(){
          if (this.sum_Chicken > 0){
            this.sum_Chicken--;
          }

      }}
  }
</script>
