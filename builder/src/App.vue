<template>
  <div class="header">
    <TheHead h1="РЕАЛИЗУЕМ КРУПНЕЙШИЕ
    ПРОЕКТЫ В РОССИИ" 
    p="стадионы, газопроводы, мосты, дамбы" show="false"></TheHead>

    <div class="number_block">
      <YearBlock number="26" text="ЛЕТ" description="на рынке"></YearBlock>
      <YearBlock number="26" text="ЛЕТ" description="на рынке"></YearBlock>
      <YearBlock number="26" text="ЛЕТ" description="на рынке"></YearBlock>
      <YearBlock number="26" text="ЛЕТ" description="на рынке"></YearBlock>
    </div>
  </div>
  

  <JustefyContentBlock Text="НАШИ САМЫЕ БОЛЬШИЕ ПРОЕКТЫ" class="fix_color" id="OurProjects">
    <ArenaBlock image-url="Data/Images/arena.png" name="Газпром Арена" description="Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву."></ArenaBlock>
    <ArenaBlock image-url="Data/Images/arena.png" name="Газпром Арена" description="Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву."></ArenaBlock>
    <ArenaBlock image-url="Data/Images/arena.png" name="Газпром Арена" description="Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия. Мы очень рады данному еву."></ArenaBlock>
  </JustefyContentBlock>

  <RequestLine h="САМЫЕ УМНЫЕ ПРОЕКТЫ" p="РЕАЛИЗУЕМ САМЫЕ СМЕЛЫЕ РЕШЕНИЯ В РОССИИ!" btn-text="ВАШ ЗАПРОС"
  @buttonclick="changeLinkShow"/>
  
  <!--Вот так нужно заполнят контент-блок-->
  <ContentBlock header="ЧЕМ МЫ ЗАНИМАЕМСЯ?" height="560px" width="1110px" style="margin-top: 30px;" id="OurWorks">
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
    <WorkLabel imageUrl="Data/Icons/building.svg" Content="Строительство офисных зданий"/>
  </ContentBlock>


  <ContentBlock height="auto">
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
    <img src="Data/Images/SomeOffice.png"/>
  </ContentBlock> 

  <div style="margin-top: 30px; margin-bottom: 60px;">
    <ContentBlock height="auto" width="900px" header="ОТВЕТЫ НА ВОПРОСЫ" vertical="true" id="Answers">
      <DropBox header="РАБОТАЕТЕ ЛИ ВЫ ПО 249 ФЗ?">
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
      <DropBox header="РАБОТАЕТЕ ЛИ ВЫ ПО 249 ФЗ?">
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
  </div>

    <!-- ----------Kirill---------- -->

  <OurPartners Text = "Наши партнеры">
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
    <AnyPartner imageUrl="Data/Images/AnyPartnerLogo.png" Content="asd" />
  </OurPartners>

  <JustefyContentBlock Text ="Отзывы о работе с нами" id="Reviews">

    <SliderComponents :Items_Array="SliderItemsReviews"/>

  </JustefyContentBlock>

  <div class="reviews_buttons">
    <div class="wrapper_content">
      <button @click="showAddElement">Оставить комментарий</button>
    </div>
  </div>

  <RequestLine h="ХОТИТЕ С НАМИ РАБОТАТЬ?" p="ОСТАВЬТЕ ЗАЯВКУ И МЫ СВЯЖЕМСЯ С ВАМИ!" btn-text="ВАШ ЗАПРОС"
  @buttonclick="changeLinkShow"/>

  <JustefyContentBlock Text ="Контакты" id="Contacts">
    <AnyContact IconUrl="Data/Icons/LocationIcon.svg" ContactName="АДРЕС:" Contact="НЕВСКИЙ ПРОСПЕКТ 140,
ОФИС 140-142"/>

    <AnyContact IconUrl="Data/Icons/PhoneIcon.svg" ContactName="ТЕЛЕФОН:" 
    Contact="8 (812) 111-22-33
8 (812) 111-22-33"/>

    <AnyContact IconUrl="Data/Icons/ClockIcon.svg" ContactName="   ВРЕМЯ РАБОТЫ:   " Contact="ПН-СБ
10:00-20:00"/>

    <AnyContact IconUrl="Data/Icons/EmailIcon.svg" ContactName="E-MAIL:" Contact="     INFO@VIP.RU     " PColor="#F7654A"
      isAddress="true" url="INFO@VIP.RU"/>
  </JustefyContentBlock>

  

  <TheFooter Campany="© 2019 строительная компания" Slogan="Разработано лучшей студией"/>

  <PopupBox Color="#F7654A" :isActive="linkPopupOn == true ? 'true' : 'false'" width="400px">
    <div :class="[inPopup.Tittle]">
      <button :class="[inPopup.Button, inPopup.ReturnButton]" @click="changeLinkShow"><img src="./assets/return.png"/></button>
      <h1 :class="[inPopup.header1]">ЗАПРОС</h1>
    </div>
    <form :class="[inPopup.form]">
      <h2 :class="[inPopup.header2]">Имя Фимилия</h2>
      <input type="text" :class="[inPopup.TextArea]" id="inputLinkName" maxlength="45" placeholder="Окулич Дмитрий Юрьевич"/>
      <h2 v-if="!popupValidateValues[0]" :class="[inPopup.headerFail]">Пустое поле</h2>

      <h2 :class="[inPopup.header2]">Электронная почта</h2>
      <input type="email" :class="[inPopup.TextArea]" id="inputLinkMail" rows="1" maxlength="45" placeholder="example@mail.com"/>
      <h2 v-if="!popupValidateValues[1]" :class="[inPopup.headerFail]">Не правильная почта!</h2>

      <h2 :class="[inPopup.header2]">Текст запроса</h2>
      <textarea type="text" :class="[inPopup.TextArea1]" id="inputLinkContent" rows="4" maxlength="300"/>
      <h2 v-if="!popupValidateValues[2]" :class="[inPopup.headerFail]">Пустое поле</h2>

      <button type="button" :class="[inPopup.Button, inPopup.ConfirmButton]" @click="confirmLink">Подтвердить</button>
    </form>
  </PopupBox>
  <PopupBox Color="#F7654A" :isActive="addElement == true ? 'true' : 'false'" width="400px">
    <div :class="[inPopup.Tittle]">
      <button :class="[inPopup.Button, inPopup.ReturnButton]" @click="showAddElement"><img src="./assets/return.png"/></button>
      <h1 :class="[inPopup.header1]">Комментарий</h1>
    </div>
    <form :class="[inPopup.form]">
      <h2 :class="[inPopup.header2]">Имя Фимилия</h2>
      <input type="text" :class="[inPopup.TextArea]" id="addProdName" maxlength="45" placeholder="Окулич Дмитрий"/>
      <h2 v-if="!addElementValidateValues[0]" :class="[inPopup.headerFail]">Пустое поле</h2>

      <h2 :class="[inPopup.header2]">Ваша компания</h2>
      <input type="text" :class="[inPopup.TextArea]" id="addProdCompany" rows="1" maxlength="45" placeholder=" ООО Газпром-Арена"/>
      <h2 v-if="!addElementValidateValues[1]" :class="[inPopup.headerFail]">Неправильное название компании</h2>

      <h2 :class="[inPopup.header2]">Текст комментария</h2>
      <textarea type="text" :class="[inPopup.TextArea1]" id="addProdComment" rows="4" maxlength="300"/>
      <h2 v-if="!addElementValidateValues[2]" :class="[inPopup.headerFail]">Пустое поле</h2>

      <button type="button" :class="[inPopup.Button, inPopup.ConfirmButton]" @click="confirmAddElements()">Подтвердить</button>
    </form>
  </PopupBox>
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
import PopupBox from './components/PopupBox.vue';

// Kirill
import OurPartners from "./components/OurPartners.vue";
import AnyPartner from "./components/AnyPartner.vue";
import AnyContact from "./components/AnyContact.vue";
import JustefyContentBlock from "./components/JustefyContentBlock.vue";
//import AnyReviews from "./components/AnyReview.vue";
import TheFooter from "./components/TheFooter.vue";
import SliderComponents from "./components/SliderComponent.vue";

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
    PopupBox,

    // Kirill
    OurPartners,
    AnyPartner,

    JustefyContentBlock,
    //AnyReviews,
    AnyContact,
    TheFooter,
    SliderComponents
  },
  methods:{
    changeLinkShow() {
      this.linkPopupOn = !this.linkPopupOn;

      this.popupValidateValues[0] = true;
      this.popupValidateValues[1] = true;
      this.popupValidateValues[2] = true;
    },
    confirmLink(){
        let nameinput : HTMLInputElement = document.getElementById('inputLinkName') as HTMLInputElement;
        let mailinput : HTMLInputElement = document.getElementById('inputLinkMail') as HTMLInputElement;
        let textcontent : HTMLTextAreaElement = document.getElementById('inputLinkContent') as HTMLTextAreaElement;

        this.popupValidateValues[0] = nameinput.value.length != 0;
        this.popupValidateValues[1] = this.IsRightMail(mailinput.value);
        this.popupValidateValues[2] = textcontent.value.length != 0;

        if (this.popupValidateValues[0] && this.popupValidateValues[1] && this.popupValidateValues[2])
          this.changeLinkShow();
    },
    IsRightMail(mail: string) : boolean {
      let reg = new RegExp('\\w+\\.?\\w*@(mail|gmail|email)\\.(com|ru|by|org)');

      return reg.test(mail);
    },
    showAddElement(){
      this.addElement = !this.addElement;

      this.addElementValidateValues[0] = true;
      this.addElementValidateValues[1] = true;
      this.addElementValidateValues[2] = true;
    },
    // Кирил! Это код обработки создания комента.
    confirmAddElements(){
        let nameinput : HTMLInputElement = document.getElementById('addProdName') as HTMLInputElement;
        let companyinput : HTMLInputElement = document.getElementById('addProdCompany') as HTMLInputElement;
        let textcontent : HTMLTextAreaElement = document.getElementById('addProdComment') as HTMLTextAreaElement;

        // Валидация

        let companyReg = new RegExp("OOO (\\w| |-|\\.)+");

        this.addElementValidateValues[0] = nameinput.value.length != 0;
        this.addElementValidateValues[1] = companyReg.test(companyinput.value);
        this.addElementValidateValues[2] = textcontent.value.length != 0;

        // Код создания элемента
        this.SliderItemsReviews.push({Id: 5, Author: "asdasdasda", Campany: "asd", Text: "asd"});
        // Тут должен быть твой код Кирил.
    }
  },
  data() {
    return {
      popupValidateValues: [false, false, false],
      linkPopupOn: false,
      addElementValidateValues: [false, false, false],
      addElement: false,

      SliderItemsReviews: [
        {Id: 1, Author: " Иванов Иван ", Campany: "ООО Газпром-Арена", Text: `Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. 
        Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. 
        В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.`},

        {Id: 2, Author: " Николай Николаевич ", Campany: "ООО Газпром-Арена", Text: `Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. 
        Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. 
        В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.`},

        {id: 3, Author: " Андреевна Анна ", Campany: "ООО Газпром-Арена", Text: `Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. 
        Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. 
        В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.`},

        {Id: 4, Author: " Петров петя ", Campany: "ООО Газпром-Арена", Text: `Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. 
        Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. 
        В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.`},

        {Id: 5, Author: " Кирилл Кириллович ", Campany: "ООО Газпром-Арена", Text: `Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. 
        Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. 
        В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов.`},
      ]
    }
  }
});
</script>

<!--Common styles-->
<style>
* {
  margin: 0;
  padding: 0;
}

.header{
  position: relative;
  height: 750px;
}

.reviews_buttons > .wrapper_content{
  display: flex;
  justify-content: flex-end;
  height: 150px;
}

.wrapper_content > button{
  width: 15%;
  height: 30%;
  background-color: #F7654A;
  border: none;
  color: white;
  font-size: 16px;
  font-family: OswaldMedium;
  cursor: pointer;
}

.number_block{
    width: 1110px;
    height: 300px;
    display: flex;
    justify-content: space-around;
    align-items:center;
    background-color: #F7F7F7;

    position: absolute;
    top: 0;
    margin-top: 490px;

    left: 50%;
    margin-left: -555px;
    
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

<!--Style modules for popup-->
<style module="inPopup">
  .Tittle {
    display: flex;

    margin-top: 15px;
  }
  .ReturnButton {
    width: 48px;
    height: 48px;

    border: solid white 1px;
    border-radius: 16px;

    justify-self: left;

    margin-left: 15px;
    margin-right: 80px;
  }
  .ReturnButton img {
    margin-top: 5px;

    width: 30px;
    height: 30px;
  }
  .ConfirmButton {
    width: 200px;
    height: 50px;

    margin-left: 80px;

    margin-top: 15px;
    margin-bottom: 15px;
  }
  .Button{
    font-family: 'OswaldBold';
    font-size: 20px;

    background: white;

    border: none;

    cursor: pointer;
  }
  .form {
    margin-left: 15px;
    margin-right: 15px;
  }
  .header1{
    font-family: 'OswaldBold';
    text-align: center;
    color: white;
  }
  .header2{
    font-family: 'OswaldBold';
    color: white;
  }

  .headerFail {
    font-family: 'OswaldBold';
    color: #DD0000;
    font-size: 16px;
  }

  .TextArea{
    width: 360px;

    margin-top: 5px;

    padding: 5px;

    border: solid black 1px;

    font-size: 16px;
    font-family: 'OswaldMedium';
  }

  .TextArea1{
    width: 360px;

    margin-top: 5px;

    resize: none;

    padding: 5px;

    border: solid black 1px;

    font-size: 16px;
    font-family: 'OswaldMedium';
  }
</style>