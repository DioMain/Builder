<template>
    <div class="dropBox_container">
        <div class="dropBox_header_container" v-on:click="Drop()">
            <img class="dropBox_header_img" src="../assets/Arrow.svg" :class="{[$style.imgdropStyle]: isDroped}"/>
            <h1 class="dropBox_header">{{ header }}</h1>
        </div>
        <div class="dropBox_content_container" v-if="isDroped">
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
            isDroped: false
        }
    },
    methods:{
        Drop() {
            this.isDroped = !this.isDroped;
        }
    }
})
</script>

<style scoped>
.dropBox_container{
    display: flex;

    flex-direction: column;
    margin-bottom: 30px;

    cursor: pointer;
}
.dropBox_header_img{
    height: 15px;
    width: 15px;

    margin-top: auto;
    margin-bottom: auto;
}
.dropBox_header{
    margin-left: 15px;
}
.dropBox_header_container{
    display: flex;

    flex-direction: row;

    font-family: "OswaldMedium";

    color: #F7654A;
}

.dropBox_header_container > h1{
    font-size: 24px;
}
.dropBox_content_container{
    display: flex;

    flex-direction: column;

    font-size: 16px;  
    font-family: "OpenSansRegular";
    
    margin-top: 15px;
    margin-bottom: 15px;

    color: #999999;
}
</style>

<style module>
.imgdropStyle{
    transform: rotateZ(90deg);
}
</style>