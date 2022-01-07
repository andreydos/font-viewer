<template>
  <div id="app">
    <div class="header">
      <div>
        <label for="input">Введите текст гравировки:</label>
        <input id="input" type="text" v-model="text" placeholder="Печатайте текст здесь">
      </div>
      <div class="logo">
        <img src="/img/logo.png" alt="GODO" width="50">
      </div>
    </div>

    <ul>
      <li v-for="(font, i) in 30" :key="i"><span class="number">{{i + 1}}.</span><span :class="`font${i + 1}`">{{text}}</span></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      text: '',
    }
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 10px;
}

.header {
  display: flex;
  align-items: center;
}

.logo {
  margin-left: 8px;
}

.number {
  margin-right: 8px;
  font-size: 24px;
  font-weight: 600;
  color: darkgray;
}

ul {
  columns: 2;
  -webkit-columns: 2;
  -moz-columns: 2;
  list-style: none;
  margin-top: 0;
  padding-left: 0;
}

@media (max-width: 550px) {
  ul {
    columns: 1;
    -webkit-columns: 1;
    -moz-columns: 1;
  }
}

input {
  width: 210px;
  height: 28px;
}

label {
  display: block;
  color: darkgrey;
}

ul li {
  display: flex;
  align-items: center;
  min-height: 50px !important;
  margin-bottom: 5px;
}

ul li span {
  line-height: 50px;
}

@font-face {
  font-family: fonts2;
  src: url("/fonts/2.ttf");
}

@font-face {
  font-family: fonts3;
  src: url("/fonts/3.ttf");
}

@font-face {
  font-family: fonts4;
  src: url("/fonts/4.ttf");
}

@font-face {
  font-family: fonts5;
  src: url("/fonts/5.ttf");
}

@font-face {
  font-family: fonts6;
  src: url("/fonts/6.ttf");
}

@font-face {
  font-family: fonts7;
  src: url("/fonts/7.ttf");
}

@font-face {
  font-family: fonts8;
  src: url("/fonts/8.ttf");
}

@font-face {
  font-family: fonts9;
  src: url("/fonts/9.ttf");
}


@font-face {
  font-family: fonts10;
  src: url("/fonts/10.ttf");
}

@font-face {
  font-family: fonts11;
  src: url("/fonts/11.ttf");
}

@font-face {
  font-family: fonts12;
  src: url("/fonts/12.ttf");
}

@font-face {
  font-family: fonts13;
  src: url("/fonts/13.ttf");
}

@font-face {
  font-family: fonts14;
  src: url("/fonts/14.ttf");
}
@font-face {
  font-family: fonts15;
  src: url("/fonts/15.ttf");
}
@font-face {
  font-family: fonts16;
  src: url("/fonts/16.ttf");
}
@font-face {
  font-family: fonts17;
  src: url("/fonts/17.ttf");
}
@font-face {
  font-family: fonts18;
  src: url("/fonts/18.ttf");
}
@font-face {
  font-family: fonts19;
  src: url("/fonts/19.ttf");
}
@font-face {
  font-family: fonts20;
  src: url("/fonts/20.ttf");
}
@font-face {
  font-family: fonts21;
  src: url("/fonts/21.ttf");
}
@font-face {
  font-family: fonts22;
  src: url("/fonts/22.ttf");
}
@font-face {
  font-family: fonts23;
  src: url("/fonts/23.ttf");
}
@font-face {
  font-family: fonts24;
  src: url("/fonts/24.ttf");
}
@font-face {
  font-family: fonts25;
  src: url("/fonts/25.ttf");
}
@font-face {
  font-family: fonts26;
  src: url("/fonts/26.otf");
}
@font-face {
  font-family: fonts27;
  src: url("/fonts/27.ttf");
}

@font-face {
  font-family: fonts28;
  src: url("/fonts/28.ttf");
}

@font-face {
  font-family: fonts29;
  src: url("/fonts/29.ttf");
}

@font-face {
  font-family: fonts30;
  src: url("/fonts/30.ttf");
}

.font1{
  height: auto;
  font-size: 30px;
}

.font2{

  height: auto;
  font-family: fonts2;
  font-size: 32px;
}

.font3{

  height: auto;
  font-family: fonts3;
  font-size: 30px;
}

.font4{

  height: auto;
  font-family: fonts4;
  font-size: 35px;
}

.font5{

  height: auto;
  font-family: fonts5;
  font-size: 37px;
}


.font6{

  height: auto;
  font-family: fonts6;
  font-size: 39px;
}


.font7{

  height: auto;
  font-family: fonts7;
  font-size: 50px;
}


.font8{

  height: auto;
  font-family: fonts8;
  font-size: 39px;
}


.font9{

  height: auto;
  font-family: fonts9;
  font-size: 44px;
}


.font10{

  height: auto;
  font-family: fonts10;
  font-size: 57px;
}


.font11{

  height: auto;
  font-family: fonts11;
  font-size: 46px;
}


.font12{

  height: auto;
  font-family: fonts12;
  font-size: 36px;
}


.font13{

  height: auto;
  font-family: fonts13;
  font-size: 49px;
}


.font14{

  height: auto;
  font-family: fonts14;
  font-size: 35px;
}


.font15{

  height: auto;
  font-family: fonts15;
  font-size: 41px;
}


.font16{

  height: auto;
  font-family: fonts16;
  font-size: 28px;
}


.font17{

  height: auto;
  font-family: fonts17;
  font-size: 39px;
}


.font18{

  height: auto;
  font-family: fonts18;
  font-size: 40px;
}


.font19{

  height: auto;
  font-family: fonts19;
  font-size: 27px;
}


.font20{

  height: auto;
  font-family: fonts20;
  font-size: 34px;
}


.font21{

  height: auto;
  font-family: fonts21;
  font-size: 41px;
}


.font22{

  height: auto;
  font-family: fonts22;
  font-size: 39px;
}


.font23{

  height: auto;
  font-family: fonts23;
  font-size: 30px;
}


.font24{

  height: auto;
  font-family: fonts24;
  font-size: 30px;
}

.font25{

  height: auto;
  font-family: fonts25;
  font-size: 32px;
}

.font26{

  height: auto;
  font-family: fonts26;
  font-size: 24px;
}

.font27{

  height: auto;
  font-family: fonts27;
  font-size: 31px;
}

.font28{

  height: auto;
  font-family: fonts28;
  font-size: 24px;
}

.font29{

  height: auto;
  font-family: fonts29;
  font-size: 31px;
}

.font30{

  height: auto;
  font-family: fonts30;
  font-size: 27px;
}
</style>
