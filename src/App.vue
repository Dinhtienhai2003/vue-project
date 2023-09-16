<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>
<script>
  export default {
    data(){
      return {
        count: 1,
      }
    },
    methods: {
      conglengmot(){
        this.count++;
      },
      trulengmot(){
        this.count--;
      }
    }
  }
</script>
<template>
  

   <p>Biến đếm: {{ count }}</p>
   <div></div>
   <button @click="conglengmot()">Cộng 1</button>
   <button @click="trulengmot()">Trừ 1</button>
   
</template>

<style scoped>
p{
  font-size: 50px;

}
button{
  font-size: 50px;
  color: rgb(237, 9, 9);
  margin: 20px;
  background-color: aqua;
}

</style>
