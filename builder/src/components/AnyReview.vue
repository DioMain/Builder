<template>
  <div class="AnyReviews_div">
        <div class="Review_Block">
            <img src="../assets/KavichkiIcon.svg" alt="">
            <!-- <slot/> -->
            <p>{{Item_Data?.Text}}</p>
        </div>  
        <div class="Author">
            <h3 class="AuthorName">{{ Item_Data?.Author }}<br><span>{{ Item_Data?.Campany }}</span></h3>
        </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'AnyReview',
    props:{
        Item_Data :{
            type: Object,
        }
    },
})
</script>

<style>
    .AnyReviews_div{
        min-width: 325px;
        margin-right: 10px;
        margin-left: 10px;
    }
    .Review_Block{
        padding: 30px;
        max-width: 265px;
        height: 290px;
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