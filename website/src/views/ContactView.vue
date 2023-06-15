<template>
    <div class="contact">
        <label for="email">Enter your email:</label>
        <input type="email" name="email" v-model="email">
        <button v-on:click="addUser()">Send</button>
    </div>
  </template>

<script>
  export default {

    data(){
        return {
          email:'',
        };
    },
    methods:{
      addUser(){
        console.warn(this.email);
      }
    }
  };


</script>


  
  <style>
 
    .contact{
      display: flex;
      align-items: center;
    }
  
  </style>