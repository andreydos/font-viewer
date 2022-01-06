<template>
  <div id="app">
    <input type="text" v-model="text">
    <div v-for="(font, i) in fonts" :key="font.cssClass" class="block">
      <p><span class="mr-8">{{i + 1}}.</span><span :class="font.cssClass">{{text}}</span></p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      text: '',
      fonts: [
        {
          cssClass: 'font-1',
          italic: true,
          thin: true
        },
        {
          cssClass: 'font-2',
          italic: true,
          thin: true
        }
      ]
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

.mr-8 {
  margin-right: 8px;
}

.font-1 {
  font-family: "Arial Black";
}

.font-2 {
  font-family: Monospaced;
}
</style>
