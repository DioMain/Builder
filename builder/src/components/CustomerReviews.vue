<template>
    <section class="Section_Reviews">
        <div class="Medium_div">
            <h2>{{ getContent() }}</h2>
            <div class="Section_Section_Reviews_Div">
                <slot/>
            </div>
        </div>
    </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'CustomerReviews',
    props:{
        Text: String
    },
    methods: {
        getContent() {
            return this.Text?.toUpperCase();
        },
    }
})
</script>

<style>
    .fix_color{
        color: #404149;
    }
    .Section_Reviews{
        height: 731px;
        width: 100%;
        background: white;
        display: flex;
        align-items: center;
    }  
    .Section_Reviews h2{
        font-size: 36px;
        padding-bottom: 60px;
        text-align: center;
        font-family: OswaldRegular;
    }  
    .Section_Section_Reviews_Div{
        max-width: 1110px;
        margin: auto;
        display: flex;
        justify-content: space-between;
    }
    .Medium_div{
        margin: auto;
        width: 1110px;
    }

</style>