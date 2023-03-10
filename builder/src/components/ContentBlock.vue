<template>
    <div class="contentBlock">
        <h1 class="contentBlock_header" :color="compColor">{{ header }}</h1>
        <div class="contentBlock_slot" :style="getSize">
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
        width: String
    },
    computed: {
        compColor() {
            return this.headerColor == "" ? "Black" : this.headerColor;
        },
        getSize(){
            return `height: ${this.height};`+
                   `width: ${this.width};`;
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
    font-family: "OswaldBold";
    font-size: 36px;

    text-align: center;
}
.contentBlock_slot{
    margin-left: auto;
    margin-right: auto;
}
</style>