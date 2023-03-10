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
        width: 100%;
        height: 20vh;
        background-color: #F7654A;
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