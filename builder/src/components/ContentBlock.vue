<template>
    <div class="wrapper_content">
        <h1 class="contentBlock_header" :color="compColor">{{ header }}</h1>
        <slot></slot>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "ContentBlock",
    props: {
        header: String,
        headerColor: String
    },
    computed: {
        compColor() {
            return this.headerColor == "" ? "Black" : this.headerColor;
        }
    }
})
</script>

<style>
.wrapper_content {
    margin-top: 10px;
}

.contentBlock_header{
    font-family: "OswaldBold";
    font-size: 36px;

    text-align: center;
}
</style>