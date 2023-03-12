<template>
    <div class="request_line">
        <div class="wrapper_content">
            <div class="request_text">
                <div class="text_content">
                    <p class="h">{{ h }}</p>
                    <p class="small">{{ p }}</p>
                </div>
            </div>
            <div class="request_button">
                <img src="../assets/buttonIcon.svg">
                <p>{{ btnText }}</p>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'RequestLine',
  props: {
    h: String,
    p: String,
    btnText: String,
  },
});
</script>

<style scoped>
    *{
        color: white;
    }
    .request_line{
        min-width: 1200px;
        width: 100%;
        height: 181px;
        background-color: #F7654A;

        margin: 150px 0 150px 0;
    }

    .request_button{
        display: flex;
        justify-content: space-around;
        align-items: center;
        background-color: white;
        width: 15%;
        height: 30%;

    }

    .request_button > p{
        font-size: 14px;
        font-family: OswaldMedium;
        color: black;
    }

    .request_button > img{
       display: block;
       width: 18px;
       height: 21px;
    }

    .wrapper_content{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .text_content{
        height: 15vh;
    }

    p{
        font-family: OswaldRegular;
        font-weight: bold;
    }
    .h{
        font-size: 48px;
    }
    .small{
        font-size: 24px;
    }
</style>