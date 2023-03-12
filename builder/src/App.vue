<template>
  <TheHead h1="РЕАЛИЗУЕМ КРУПНЕЙШИЕ
  ПРОЕКТЫ В РОССИИ" 
  p="стадионы, газопроводы, мосты, дамбы"></TheHead>
  <YearBlock number="26" text="ЛЕТ" description="на рынке"></YearBlock>

  <CustomerReviews Text="НАШИ САМЫЕ БОЛЬШИЕ ПРОЕКТЫ">
    <ArenaBlock image-url="Data/Images/arena.png" name="Газпром Арена" description="Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву."></ArenaBlock>
    <ArenaBlock image-url="Data/Images/arena.png" name="Газпром Арена" description="Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву."></ArenaBlock>
    <ArenaBlock image-url="Data/Images/arena.png" name="Газпром Арена" description="Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву."></ArenaBlock>
  </CustomerReviews>

  <RequestLine h="САМЫЕ УМНЫЕ ПРОЕКТЫ" p="РЕАЛИЗУЕМ САМЫЕ СМЕЛЫЕ РЕШЕНИЯ В РОССИИ!" btn-text="ВАШ ЗАПРОС"></RequestLine>
  
  <!--Вот так нужно заполнят контент-блок-->
  <ContentBlock header="ЧЕМ МЫ ЗАНИМАЕМСЯ?" height="639px" width="1110px">
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

  <ContentBlock height="500px" width="900px" header="ОТВЕТЫ НА ВОПРОСЫ" style="margin-top: 50px;">
    <DropBox header="РАБОТАЕТЕ ЛИ ВЫ ПО 249 ФЗ?" style="margin-top: 25px;">
      <div>
        Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem Ipsum является стандартной 
        "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный печатник создал большую коллекцию 
        размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов.
      </div>
    </DropBox>
    <DropBox header="РАБОТАЕТЕ ЛИ ВЫ ПО 249 ФЗ?">
      <div>
        Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem Ipsum является стандартной 
        "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный печатник создал большую коллекцию 
        размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов.
      </div>
    </DropBox>
  </ContentBlock>

    <!-- ----------Kirill---------- -->

  <OurPartners Text = "Наши партнеры">
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
  </OurPartners>

  <CustomerReviews Text ="Отзывы о работе с нами">
    <AnyReviews Author="Иванов Иван, " Campany="ООО Газпром-Арена">
      <p>Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. 
        Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. 
        В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.</p>
    </AnyReviews>
    <AnyReviews Author="Иванов Иван, " Campany="ООО Газпром-Арена">
      <p>Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. 
        Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. 
        В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.</p>
    </AnyReviews>
    <AnyReviews Author="Иванов Иван, " Campany="ООО Газпром-Арена">
      <p>Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. 
        Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. 
        В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.</p>
    </AnyReviews>
  </CustomerReviews>

  <RequestLine h="ХОТИТЕ С НАМИ РАБОТАТЬ?" p="ОСТАВЬТЕ ЗАЯВКУ И МЫ СВЯЖЕМСЯ С ВАМИ!" btn-text="ВАШ ЗАПРОС"></RequestLine>

</template>

<script lang="ts">
import { defineComponent } from 'vue';

import TheHead from './components/TheHead.vue';
import RequestLine from './components/Request.vue';
import WorkLabel from './components/WorkLabel.vue';
import ContentBlock from './components/ContentBlock.vue';
import YearBlock from './components/YearBlock.vue';
import DropBox from './components/DropBox.vue';
import ArenaBlock from './components/ArenaBlock.vue';

// Kirill
import OurPartners from "./components/OurPartners.vue";
import AnyPartner from "./components/AnyPartner.vue";

import CustomerReviews from "./components/CustomerReviews.vue";
import AnyReviews from "./components/AnyReview.vue";

export default defineComponent({
  name: 'App',
  components: {
    TheHead,
    RequestLine,
    WorkLabel,
    ArenaBlock,
    YearBlock,
    ContentBlock,
    DropBox,

    // Kirill
    OurPartners,
    AnyPartner,

    CustomerReviews,
    AnyReviews
  }
});
</script>

<style>
* {
  margin: 0;
  padding: 0;

}

.wrapper_content{
    width: 1110px;
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
