<template>
    <header>
        <div class="wrapper_content">
            <div class="header_menu" id="Head">
                <a href="#"><img src="../assets/logo.svg" alt="menu logo"></a>
                <div class="menu_burger"  @click="show = !show">
                    <img src="../assets/burgerMenu.svg" alt="">
                </div>
                <nav  class="menu_nav" v-if="show">
                    <ul class="menu_list">
                        <li><a href="#Head" class="menu__item">Главная</a></li>
                        <li><a href="#OurProjects" class="menu__item">Проекты</a></li>
                        <li><a href="#OurWorks" class="menu__item">Наши направления</a></li>
                        <li><a href="#Answers" class="menu__item">Ответы на вопросы</a></li>
                        <li><a href="#Reviews" class="menu__item">Отзывы</a></li>
                        <li><a href="#Contacts" class="menu__item">Контакты</a></li>
                    </ul>
                </nav>
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
    p: String
  },
  data() {
        return {
            show: false,
        }
    }
});
</script>

<style scoped>
header{
    min-width: 1200px;
    width: 100%;
    height: 640px;
    background-image: url(../assets/Header.png);
    background-size: cover;
    color: white;
}

.menu_nav{
    background-color: #404149;
    position: absolute;
    right: 0;
    margin-top: 55px;
    font-size: 25px;
    color: white;
    font-family: OswaldMedium;
    border-left: 10px solid #F7654A;
}

.menu_nav > ul{
    list-style: none;
}

.menu_nav > ul > li{
    margin: 10px 25px 10px 25px;
}

.menu_nav > ul > li > a{
    text-decoration: none;
    color: white;
}

.menu_nav a:hover{
    color: gray;
}
.header_menu{
    position: relative;
    padding-top: 30px;
    padding-bottom: 80px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.header_menu img{
    display: block;
}

.menu_burger{
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #F7654A;
    width: 50px;
    height: 50px;

    align-self: center;
}

.menu_burger:hover{
    cursor: pointer;
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