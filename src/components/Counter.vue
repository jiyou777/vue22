<template>
    <div>
        <button @click="increment">+</button>
        <button v-on:click="decrement">-</button>
        123123
        <p><span>{{num}}</span></p>
    </div>
</template>
<style>
</style>
<script>
    export default{
        props:["num"],
        data(){
            return{
            }
        },
        methods:{
          increment(){
            this.$emit("incre");
          },
          decrement(){
            this.$emit("decre");
          }
        }
    }
</script>
