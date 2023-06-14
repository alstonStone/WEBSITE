<template>
    <div class="contact">
        <form action="http://localhost:7070/contact">
            <label for="email">Enter your email:</label>
            <input type="email" id="email" name="email">
            <input type="submit" value="Submit">
        </form>
    </div>
  </template>
  
  <style>
 
    .contact{
      display: flex;
      align-items: center;
    }
  
  </style>