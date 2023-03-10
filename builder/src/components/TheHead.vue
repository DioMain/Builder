<template>
    <header>
        <div class="header_content">
            <div class="header_menu">
                <img src="../assets/logo.svg" alt="menu logo">
                <div class="menu_burger"></div>
            </div>
            <div class="header_text">
                <pre>{{ h1 }}</pre>
                <p>{{ p }}</p>
            </div>
        </div>
    </header>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'TheHead',
  props: {
    h1: String,
    p: String,
  },
});
</script>

<style scoped>
header{
    width: 100%;
    background-image: url(../assets/Header.png);
    background-size: cover;
    height: 30vh;
    color: white;
}
.header_content{
    width: 60%;
    margin: 0 auto 0 auto;
}
.header_menu{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.header_menu img{
    display: block;
}

.menu_burger{
    background-color: #F7654A;
}

pre, p{
    text-align: center;
}

pre{
    font-size: 64px;
    font-weight: bolder;
}

p{
    font-size: 18px;
}

</style>