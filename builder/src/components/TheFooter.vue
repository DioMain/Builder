<template>
    <footer class="Footer">
        <div>
            <p>{{ Campany }}</p>
            <p>{{ Slogan }}</p> 
        </div>       
    </footer>
  </template>
  
  <script lang="ts">
  import { defineComponent } from 'vue';
  
  export default defineComponent({
      name: 'TheFooter',
      props:{
        Campany: String,
        Slogan: String,
      },
  })
  </script>
  
  <style>

  footer{
    height: 80px;
    background: #404149;
    display: flex;
    align-items: center;
  }
  footer p{
    color: white;
    font-size: 15px;
    font-family: OpenSansRegular;
}
  footer div{
    width: 1110px;
    margin: auto;
    display: flex;
    justify-content: space-between;
  }
  
  </style>