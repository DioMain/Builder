<template>
    <div class="PopupBox_main" v-if="isActive == 'true'">
        <div class="PopupBox_bg"></div>
        <main class="PopupBox_container" :style="getContainerStyle">
            <slot></slot>
        </main>
    </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "PopupBox",
    props: {
        Color: String,
        isActive: String
    },
    computed: {
        getContainerStyle() {
            return `background-color: ${this.Color == undefined ? "white" : this.Color};`+
                    `border: solid ${this.Color == undefined ? "white" : this.Color} 6px;`;
        }
    }
})
</script>

<style>
.PopupBox_main {
    position: fixed;

    left: 0;
    top: 0;

    animation: shadebgin ease-in 0.25s;

    width: 100%;
    height: 100%;
}
.PopupBox_bg {
    position: fixed;

   
    opacity: 0.4;

    background-color: black;

    left: 0;
    top: 0;

    width: 100%;
    height: 100%;

    animation: capacity 0.2;
}
.PopupBox_container{
    position: relative;

    border-radius: 24px;

    margin-left: auto;
    margin-right: auto;

    width: fit-content;

    font-family: "OswaldMedium";
    font-size: 16px;

    top: 50%;
    transform: translateY(-50%);
}

@keyframes shadebgin {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}
</style>