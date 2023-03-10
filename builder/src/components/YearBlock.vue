<template>
    <div class="year_block">
        <div class="block_number">{{ number }}</div>
        <div class="block_text">{{ text }}</div>
        <div class="block_description">{{ description }}</div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'YearBlock',
  props: {
    number: String,
    text: String,
    description: String
  }
});
</script>

<style scoped>
    .year_block{
        width: 190px;
    }
    .block_number{
        font-size: 72px;
        font-family: OswaldMedium;
        color: #F7654A;
        text-align: center;
    }

    .block_text{
        font-size: 36px;
        font-family: OswaldMedium;
        color: #000000;
        text-align: center;
    }

    .block_description{
        font-size: 18px;
        font-family: OswaldMedium;
        color: #999999;
        text-align: center;
    }
</style>