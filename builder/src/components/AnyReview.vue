<template>
  <div>
        <div class="Review_Block">
            <img src="../assets/KavichkiIcon.svg" alt="">
            <slot/>
        </div>  
        <div class="Author">
            <h3 class="AuthorName">{{ Author }}<span>{{ Campany }}</span></h3>
        </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'AnyReview',
    props:{
        Author: String,
        Campany: String
    },
})
</script>

<style>
    .Review_Block{
        padding: 30px;
        max-width: 290px;
        max-height: 290px;
        background: #F7F7F7;
    }
    .Review_Block p{
        font-size: 15px;
        padding: 20px 0 20px 0;
        font-family: OpenSansRegular;
    }
    .Author{
        padding-top: 30px;
    }
    .AuthorName{
        font-size: 20px;
        font-family: OpenSansRegular;

    }
    .AuthorName span{
        color: #F7654A;
    }
</style>