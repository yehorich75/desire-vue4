<template>
  <div class="wrapper">
    <Header>
      <HeaderInner />
    </Header>
    <Main />
  </div>
</template>

<script>
  import { defineComponent } from 'vue'
  import Header from './components/Header.vue'
  import HeaderInner from './components/HeaderInner.vue'
  import Main from './components/Main.vue'

  export default defineComponent({
    name: 'App',
    components: {
      Header,
      HeaderInner,
      Main
    }
  })
</script>



<style>

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html,
body {
  height: 100%;
}

html {
  font-size: 10px;
}

body {
  font-family: 'Open Sans', sans-serif;
  font-size: 1.6rem;
  line-height: 2.7rem;
  font-weight: 400;
  color: #5A5A5A;
  overflow-x: hidden;
  min-width: 32rem;
}

.wrapper {
  display: flex;
  flex-direction: column;
  min-height: 100%;
}

.main {
  flex: 1 0 auto;
}
.footer {
  flex: 0 0 auto;
}

.container {
  max-width: 1140px;
  margin: 0 auto;
  padding: 0 15px;
}

.container-fluid {
  max-width: 192rem;
  margin: 0 auto;
  padding: 0 1rem;
}

.slick-dots {
  display: flex;
  justify-content: center;
  align-items: center;
}

.slick-dots button {
  width: 8px;
  height: 8px;
  background-color: #363838;
  border: none;
  border-radius: 4px;
  margin: 0 15px;
  font-size: 0;
}

.slick-dots li.slick-active button {
background-color: #f1d152;
}

</style>

