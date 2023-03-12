<template>
    <section class="Section_Partners">
        <h2>{{ getContent() }}</h2>
        <div class="Section_Partners_Div">
            <slot/>
        </div>
    </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'OurPartners',
    props:{
        Text: String,
    },
    methods: {
        getContent() {
            return this.Text?.toUpperCase();
        }
    }
})
</script>

<style>
    .Section_Partners{
        background: #404149;
        height: 300px;
    }
    .Section_Partners h2{
        text-align: center;
        padding: 60px;
        font-size: 35px;
        color: white;
        font-family: OswaldRegular;
    }
    .Section_Partners_Div{
        width: 1110px;
        margin: auto;

        display:  flex;
        justify-content: space-between;
    }
</style>