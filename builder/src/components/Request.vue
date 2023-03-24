<template>
    <div class="request_line">
        <div class="wrapper_content">
            <div class="request_text">
                <div class="text_content">
                    <p class="h">{{ h }}</p>
                    <p class="small">{{ p }}</p>
                </div>
            </div>
            <button class="request_button" @click="buttonClick()">
                <img src="../assets/buttonIcon.svg">
                <p>{{ btnText }}</p>
            </button>
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
    btnText: String
  },
  methods: {
    buttonClick(){
        this.$emit('buttonclick');
    }
  }
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

    }

    .request_button{
        display: flex;
        justify-content: space-around;
        align-items: center;
        background-color: #F7654A;
        width: 15%;
        height: 30%;

        border: 1px solid black;
        overflow: hidden;
        position: relative;
    }

    .request_button:active{
        transform: scale(0.99);
    }

    .request_button:after {
        background: #fff;
        content: "";
        height: 155px;
        left: -75px;
        opacity: .2;
        position: absolute;
        top: -50px;
        transform: rotate(35deg);
        transition: all 550ms cubic-bezier(0.19, 1, 0.22, 1);
        width: 50px;
    }

    .request_button:hover:after {
        left: 120%;
        transition: all 550ms cubic-bezier(0.19, 1, 0.22, 1);
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

    .request_button:hover {
        cursor:pointer;
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