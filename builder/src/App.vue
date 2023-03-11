<template>
  <TheHead h1="РЕАЛИЗУЕМ КРУПНЕЙШИЕ
  ПРОЕКТЫ В РОССИИ" 
  p="стадионы, газопроводы, мосты, дамбы"></TheHead>
  <YearBlock number="26" text="ЛЕТ" description="на рынке"></YearBlock>
  <RequestLine h="САМЫЕ УМНЫЕ ПРОЕКТЫ" p="РЕАЛИЗУЕМ САМЫЕ СМЕЛЫЕ РЕШЕНИЯ В РОССИИ!" btn-text="ВАШ ЗАПРОС"></RequestLine>
  
  <!--Вот так нужно заполнят контент-блок-->
  <ContentBlock header="ЧЕМ МЫ ЗАНИМАЕМСЯ?" height="500px" width="900px">
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
  </ContentBlock>

  <ContentBlock height="650px">
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
  </ContentBlock> 
  <!-- <ArenaBlock image-url="Data/Images/arena.png" name="Газпром Арена" description="Мы сделали самую красивую арену в Европе.
                                   Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. 
                                   Мы очень рады данному еву.">
  </ArenaBlock> -->


  <!--Зона Кирилла-->
<OurPartners/>

</template>

<script lang="ts">
import { defineComponent } from 'vue';
import TheHead from './components/TheHead.vue';
import RequestLine from './components/Request.vue';
import WorkLabel from './components/WorkLabel.vue';
import ContentBlock from './components/ContentBlock.vue';
import YearBlock from './components/YearBlock.vue';
// import ArenaBlock from './components/ArenaBlock.vue';

// Kirill
import OurPartners from "./components/OurPartners.vue";

export default defineComponent({
  name: 'App',
  components: {
    TheHead,
    RequestLine,
    WorkLabel,
    // ArenaBlock,
    YearBlock,
    ContentBlock,

    // Kirill
    OurPartners
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
