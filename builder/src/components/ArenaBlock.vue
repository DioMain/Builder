<template>
    <div class="project_card">
        <img class="card_image" :src="imageUrl" alt="card image">
        <div class="card_line"></div>
        <p class="card_name">{{ name }}</p>
        <p class="card_description">{{ description }}</p>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ArenaBlock',
  props: {
    imageUrl: String,
    name: String,
    description: String
  }
});
</script>

<style scoped>
    .project_card{
        width: 350px;
    }
    .card_line{
        width: 60px;
        height: 6px;
        background-color: #F7654A;

        margin-top: 30px;
        margin-bottom: 15px;
    }
    .card_name{
        font-family: OswaldMedium;
        font-size: 24px;
        color: #404149;
    }

    .card_description{
        font-family: OpenSansRegular;
        font-size: 16px;
        color: #999999;
    }
    
    .card_image{
        width: 100%;
    }
</style>