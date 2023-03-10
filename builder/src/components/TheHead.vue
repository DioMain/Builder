<template>
    <header>
        <div class="wrapper_content">
            <div class="header_menu">
                <a href="#"><img src="../assets/logo.svg" alt="menu logo"></a>
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
    min-width: 1200px;
    width: 100%;
    background-image: url(../assets/Header.png);
    background-size: cover;
    height: 50vh;
    color: white;
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
    width: 50px;
    height: 50px;

    align-self: center;
}

pre, p{
    text-align: center;
}

pre{
    font-size: 64px;
    font-family: OswaldMedium;
}

p{
    font-size: 18px;
    font-family: OswaldRegular;
}

</style>