<template>
    <div class="dropBox_container">
        <div class="dropBox_header_container" >
            <img class="dropBox_header_img" src="../assets/Arrow.svg" v-on:click="Drop()" :style="imgDropStyle"/>
            <h1 class="dropBox_header">{{ header }}</h1>
        </div>
        <div class="dropBox_content_container" :style="containerDropStyle">
            <slot/>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "DropBox",
    props:{
        header: String
    },
    data(){
        return{
            isDroped: false,
            containerDropStyle: "",
            imgDropStyle: ""
        }
    },
    methods:{
        Drop() {
            if (this.isDroped){
                this.containerDropStyle = "display: flex;";
                this.imgDropStyle = "transform: rotateZ(90deg);";
            }               
            else{
                this.containerDropStyle = "display: none;";
                this.imgDropStyle = "transform: rotateZ(0deg);";
            } 
                

            this.isDroped = !this.isDroped;
        }
    }
})
</script>

<style>
.dropBox_container{
    display: flex;

    flex-direction: column;
}
.dropBox_header_img{
    height: 25px;
    width: 25px;

    margin-top: auto;
    margin-bottom: auto;

    transform: rotateZ(0deg);
}
.dropBox_header{
    margin-left: 15px;
}
.dropBox_header_container{
    display: flex;

    flex-direction: row;

    font-size: 20px;
    font-family: "OswaldMedium";

    color: #F7654A;
}
.dropBox_content_container{
    display: none;

    flex-direction: column;

    font-size: 16px;  
    font-family: "OpenSansRegular";
    
    margin-top: 30px;
    margin-bottom: 30px;

    color: #999999;
}
</style>