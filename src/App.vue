<template>
  <div id="app">
    <!-- <my-button></my-button> -->
    <!-- <set-time-button :time='60' :startMsg="message"></set-time-button> -->
    <button-set-time :time="60"></button-set-time>
    <div v-html="md"></div>

  </div>
</template>

<script>

// import myButton from "./components/button";
// import setTimeButton from "./components/buttonSetTime";




import templatename from './template.md'
export default {
  name: "App",
  components: {
  //   myButton,
  //   setTimeButton,
  //   // buttonTime
  // buttonsettime
  },
  data() {
    return {
      message:'点我获取信息。。。。',
      md:templatename
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
