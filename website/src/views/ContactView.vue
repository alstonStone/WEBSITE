<template>
    <div class="contact">
        <label for="email">Enter your email:</label>
        <input type="email" name="email" v-model="email">
        <button v-on:click="addUser()">Send</button>
    </div>
  </template>

<script>
  import axios, {isCancel, AxiosError} from 'axios';
  export default {

    
    data(){
        return {
          email:''
        };
    },
    methods:{
      async addUser(){
        let result =  await axios.post("http://localhost:7070/contact",
        {email:this.email},{withCredentials: false}
        );
        console.warn(result);
      },
    },
  };


</script>


  
  <style>
 
    .contact{
      display: flex;
      align-items: center;
    }
  
  </style>