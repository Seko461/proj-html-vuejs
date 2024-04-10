<script >
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style >
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200..700&family=Roboto+Condensed:ital,wght@0,100..900;1,100..900&display=swap');


* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Oswald", sans-serif;
  font-optical-sizing: auto;
  font-weight: 400;

  font-style: normal;

}


body {
  overflow: auto;
  overflow-x: hidden;
  max-width: 1450px;
  margin: auto;
  position: relative;

}

::-webkit-scrollbar {
  display: none;
}
</style>
