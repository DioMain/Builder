<template>
    <div class="Contact_Div_img">
        <img :src="IconUrl" alt="Icon">
        <h3>{{ ContactName }}</h3>
        <pre>{{ Contact }}</pre>
    </div>
  </template>
  
  <script lang="ts">
  import { defineComponent } from 'vue';
  
  export default defineComponent({
      name: 'AnyContact',
      props:{
        IconUrl: String,
        ContactName: String,
        Contact: String
      },
  })
  </script>
  
  <style>
  .Contact_Div_img{
        text-align: center;
        font-size: 26px;
    }
    .Contact_Div_img img{
        padding: 20px;
        width: 50px;
        height: 50px;
    }
    .Contact_Div_img pre{
        padding-top: 20px;
        font-family: "OswaldMedium";
    }
    .Contact_Div_img h3{
        color: rgb(158, 158, 158);
        padding-top: 20px;
        font-family: OswaldRegular;
        font-weight: normal;
    }
  
  </style>