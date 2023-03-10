<template>
    <div class="workLabel_container">
        <div class="workLabel_icon_container">
            <img class="workLabel_icon" :src="imageUrl"/>
        </div>

        <p class="workLabel_content">{{ getContent() }}</p>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'WorkLabel',
    props:{
        imageUrl: String,
        Content: String,
    },
    methods: {
        getContent() {
            return this.Content?.toUpperCase();
        }
    }
})
</script>

<style>
    .workLabel_container {
        font-family: 'OswaldBold';
        font-size: 21px;

        float: left;
        
        margin-top: 15px;
        margin-left: 15px;

        width: 275px;
        height: 200px;
        
        background-color: #F7F7F7;
    }
    .workLabel_content{
        text-align: center;
        width: auto;

        margin-top: 15px;
    }
    .workLabel_icon_container{
        width: 60px;
        height: 40px;

        margin-left: auto;
        margin-right: auto;
        margin-top: 65px;
    }
    .workLabel_icon{
        color: #F7654A;
        border: #F7654A;
        fill: #F7654A;
        

        width: 60px;
        height: 40px;
    }
</style>