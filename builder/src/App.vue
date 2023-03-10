<template>
  <TheHead h1="РЕАЛИЗУЕМ КРУПНЕЙШИЕ
  ПРОЕКТЫ В РОССИИ" 
  p="стадионы, газопроводы, мосты, дамбы"></TheHead>
  <YearBlock number="26" text="ЛЕТ" description="на рынке"></YearBlock>
  <RequestLine h="САМЫЕ УМНЫЕ ПРОЕКТЫ" p="РЕАЛИЗУЕМ САМЫЕ СМЕЛЫЕ РЕШЕНИЯ В РОССИИ!" btn-text="ВАШ ЗАПРОС"></RequestLine>
  
  <!--Вот так нужно заполнят контент-блок-->
  <ContentBlock header="Some text" height="500px" width="900px">
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Some text"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Some text"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Some text"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Some text"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Some text"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Some text"/>
  </ContentBlock>
  <!-- <ArenaBlock image-url="Data/Images/arena.png" name="Газпром Арена" description="Мы сделали самую красивую арену в Европе.
                                   Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. 
                                   Мы очень рады данному еву.">
  </ArenaBlock> -->
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import TheHead from './components/TheHead.vue';
import RequestLine from './components/Request.vue';
import WorkLabel from './components/WorkLabel.vue';
import ContentBlock from './components/ContentBlock.vue';
import YearBlock from './components/YearBlock.vue';
// import ArenaBlock from './components/ArenaBlock.vue';

export default defineComponent({
  name: 'App',
  components: {
    TheHead,
    RequestLine,
    WorkLabel,
    // ArenaBlock,
    YearBlock,
    ContentBlock
  }
});
</script>

<style>
* {
  margin: 0;
  padding: 0;

}

.wrapper_content{
    width: 60%;
    height: 100%;
    margin: 0 auto 0 auto;
}

@font-face {
  font-family: "OpenSansRegular";
  src:url(../src/assets/fonts/OpenSans-Regular.ttf);
  font-style: normal;
  font-weight: normal;
}

@font-face {
  font-family: "OswaldRegular";
  src:url(../src/assets/fonts/Oswald-Regular.ttf);
  font-style: normal;
  font-weight: normal;
}

@font-face {
  font-family: "OswaldMedium";
  src:url(../src/assets/fonts/Oswald-Medium.ttf);
  font-style: normal;
  font-weight: normal;
}

@font-face {
  font-family: "OswaldBold";
  src:url(../src/assets/fonts/Oswald-Bold.ttf);
  font-style: normal;
  font-weight: normal;
}
</style>
