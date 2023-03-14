<template>
    <div class="Slider_div">
        <button class="Slider_Button">
            <img src="../assets/keyboard-left.svg" alt="">
        </button>
        <div class="Whithout_Buttom">
            <AnyReview 
            v-for="Item in Items_Array"
            :key="Item.id"
            :Item_Data="Item"
        />
        </div>
        <button class="Slider_Button">
            <img src="../assets/keyboard-right.svg" alt="">
        </button>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import AnyReview from './AnyReview.vue';
  
  export default defineComponent({
    name: "AnyContact",
    props: {
        Items_Array: {
            type: Array,
            default: () => []
        },
        SlideIndex : Number
        
    },
    computed: {
    // h3Style() {
    //     return `color: ${this.PColor == "" ? "#000000" : this.PColor}`;
    // },
    // getUrl() {
    //     return this.url == undefined ? "" : `mailto:${this.url}`;
    // }
    },
    components: { AnyReview }
})
</script>

<style>
    .Slider_Button{
        height: 40px;
        border: none;
        background: none;   
        margin-top: -80px;     
    }
    .Slider_Button img{
        width: 40px;
    }
    .Slider_div{
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .Whithout_Buttom{
        width: 1110px;
        margin: auto;
        display: flex;
        justify-content: space-between;
        overflow: hidden;
    }
</style>