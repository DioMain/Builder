<template>
    <div class="contentBlock">
        <h1 class="contentBlock_header" :style="headerStyle">{{ header }}</h1>
        <div class="contentBlock_slot" :style="getContainerStyle">
            <slot/>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "ContentBlock",
    props: {
        header: String,
        headerColor: String,
        height: String,
        width: String,
        vertical: String
    }, 
    computed: {
        headerStyle() {
            return `color: ${this.headerColor == "" ? "#000000" : this.headerColor}`;
        },
        getContainerStyle(){
            return `height: ${this.height == "" ? "auto" : this.height};`+
                   `width: ${this.width == "" ? "auto" : this.width};` +
                   `flex-direction: ${this.vertical == "true" ? "column" : "row"};`;
        }
    }
})
</script>

<style>
.contentBlock{
    margin-top: 10px;

    width: 100%;
}
.contentBlock_header{
    padding-bottom: 60px;

    font-family: "OswaldBold";
    font-size: 36px;

    text-align: center;
}
.contentBlock_slot{
    margin-left: auto;
    margin-right: auto;
    
    justify-content: space-between;

    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}
.contentBlock_slot > img {
    width: 25%;
}
</style>