<template>
    <div class="Partner_Div_logo">
        <img class="PartnerImgLogo" :src="imageUrl" :alt="Content">
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'AnyPartner',
    props:{
        imageUrl: String,
        Content: String,
    },
})
</script>

<style>
    .Partner_Div_logo{
        max-width: 170px;
        max-height: 61px;
    }
    .Partner_Div_logo img{
        max-width: 100%;
        max-height: 100%;
    }
</style>