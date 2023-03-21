<template>
    <div class="Slider_div">
        <button class="Slider_Button Left_Button" @click="PredSlide">
            <img src="../assets/keyboard-left.svg" alt="">
        </button>
        <div class="Whithout_Buttom">
            <div class="Slider_Button_Div" :style="{'margin-left': '-' + (345 * SlidePosition) + 'px'}">
                <AnyReview 
                    v-for="Item in Items_Array"
                    :key="Item.id"
                    :Item_Data="Item"
                />
            </div>
        </div>
        <button class="Slider_Button" @click="NextSlide">
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
    components: 
    {
         AnyReview 
    },
    methods:{
        PredSlide(){
            if(this.SlidePosition > 0){
                this.SlidePosition--;
                //console.log(this.SlidePosition);
            }
        },
        NextSlide(){
            if(this.SlidePosition < (this.Items_Array.length - 3)){
                this.SlidePosition++;
                //console.log(this.SlidePosition);
            }
        }
    },
    data(){
        return {
            SlidePosition: 0
        }
    }
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
        fill: #F7654A;
    }
    .Slider_div{
        max-width: 1110px;
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
    .Slider_Button_Div{
        width: 1110px;
        margin: auto;
        display: flex;
        justify-content: space-between;
    }
</style>